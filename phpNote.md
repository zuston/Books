## php——————note

- ##### object traits
  
  1. parent（指向父对象的方法和常量）
     
     > parent::__construct();
     > 
     > $this->count=parent::$count;
     
  2. self（指向类本身，一般用于静态常量的调用）
     
     静态常量存在于一次生命周期的内存中，跟每一个对象实例无关，只跟调用的类相关，内存中关于这个类只存在一个$count
     
     > ``` 
     > public static $count = 0;
     > public function getCount(){
     > 	return self::$count;
     > }
     > ```
     
  3. this（指向实例化的对象）
     
     是属于实例化对象的每一个成员属性，跟实例化对象有关
     
     > ``` 
     > public $count = 0;
     > public function getCount(){
     > 	return $this->count;
     > }
     > ```
  
- ​