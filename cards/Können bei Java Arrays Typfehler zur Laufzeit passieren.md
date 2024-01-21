

Können bei Java Arrays Typfehler zur Laufzeit passieren?

Ja:
class Loophole {
public static String loophole(Integer y) {
String[] xs = new String[10];
Object[] ys = xs; // no compile-time error
ys[0] = y; // throws ArrayStoreException
return xs[0];
} }

