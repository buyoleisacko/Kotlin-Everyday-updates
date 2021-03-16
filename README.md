# Kotlin-Everyday-updates


Kotlin Data Types:

Kotlin has the following basic data types:
Boolean
Char
Byte
Short
Int
Long
Float
Double
Array

Kotlin Boolean values
In Kotlin the boolean data type is a primitive data type having one of two values: true or false.

Example:

fun main() {

    var name = ""
    val male: Boolean = Random.nextBoolean()

    if (male) {
        name = "Robert"
    }

    if (!male) {
        name = "Victoria"
    }

    println("We will use name $name")

    println(9 > 8)
}
Kotlin integers:
Integers are a subset of the real numbers. They are written without a fraction or a decimal component. Integers fall within a set Z = {..., -2, -1, 0, 1, 2, } Integers are infinite.

The usage of integers depends on the type of the task we have. 
All variables initialized with integer values not exceeding the maximum value of Int have the inferred type Int. 
If the initial value exceeds this value, then the type is Long. To specify the Long value explicitly, append the suffix L to the value.
When we work with integers, we deal with discrete items.
Kotlin integer min/max values:
The integer data types provide their min and max values as constants.

Kotlin BigInteger:
Byte, Short, Int and Long types are used to represent fixed precision numbers. This means that they can represent a limited amount of integers. 

We print the largest integer value which can be represented by the Long type. Example:
val b = BigInteger("92233720368547758071")
val c = BigInteger("52498235605326345645")

We define two BigInteger objects. They both hold larger values that a Long type can hold.
val a = b.multiply(c)

Kotlin arithmetic overflow:
An arithmetic overflow is a condition that occurs when a calculation produces a result that is greater in magnitude than that which a given register or storage location can store or represent.
When we try to assign a value beyond the range of a data type. This leads to an arithmetic overflow. When an overflow occurs, the variable is reset to a negative upper range value.
Example:
fun main() {

    var a: Byte = 126

    println(a)
    a++

    println(a)
    a++

    println(a)
    a++

    println(a)
}

Kotlin floating point numbers:
Real numbers measure continuous quantities, like weight, height, or speed. Floating point numbers represent an approximation of real numbers in computing. In Kotlin we have two primitive floating point types: Float and Double. The Float is a single precision type which stores numbers in 32 bits. The Double is a double precision type which stores numbers in 64 bits.
Example:
fun main() {

    val speed: Float

    val distance = 0.1f
    val time: Float = 9.87f / 3600

    speed = distance / time

    println("The average speed of a sprinter is $speed km/h")
}

We use the DecimalFormat class to arrange our double value into standard decimal format.
val bd = BigDecimal("1.212e-19")

println(bd.toEngineeringString())
println(bd.toPlainString())

Kotlin explicit conversions:
Kotlin supports explicit conversion between numbers.
Every number type has the following conversion functions:
toByte(): Byte
toShort(): Short
toInt(): Int
toLong(): Long
toFloat(): Float
toDouble(): Double
toChar(): Char
Kotlin strings and chars:
A String is a data type representing textual data in computer programs. A string in Kotlin is a sequence of characters. A Char is a single character. Strings are enclosed by double quotes.

Kotlin Arrays:
Array is a complex data type which handles a collection of elements. Each of the elements can be accessed by an index. All the elements of an array must be of the same data type.

Single line Expressions in Kotlin;

