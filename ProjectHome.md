Persister is an ORM library for PHP. It allows users to easily perform CRUD functions on a PHP object. Here is some example code:

$p = new persister('className'); // where className is the name of the class for which you wish to create a persister object

$p->load($obj); // where $obj is an object of className and this function will load up all the properties of $obj from the DB

echo $obj->name; // access the properties normally

$obj->score = 50;

$p->save($obj); // persist the properties of the object back to DB

XML mapping files are utilized for the ORM. Several more functions are possible and will be documented at a later time.