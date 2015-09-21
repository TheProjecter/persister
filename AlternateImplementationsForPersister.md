lternate implementation1: (g)

class user extends persister { .... }

$u = new user();

$u->save();

user->fetchmembers(); //breaks semantics unless static



Alternate implementation2:


$p = new persister("user"); //pass class name as string

$u = new user(23);

$p->load($u);

$u2 = new user();

$u2->arr[x](x.md) = 2;

$p->save($u2);

$p->fetchmembers();

$c = new category();

$p->save($c); // throws exception!

$p->delete($u3); // record disappears from table and u3 becomes null


Alternate implementation3:


class user { persister $p; function construct() { $p = new persister(); } }


$u = new user();

$u->$p->save();