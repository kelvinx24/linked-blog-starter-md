Problem: We want to be able to configure an object on creation and
	1) the constructor is way too long
	2) we are constrained and cannot create the constructors we need

Solution : To make a class with the purpose of customizing and creating our object (Builder)

1) Create a class Builder with fields that mirror the implementation
2) In this class Builder, create a constructor that sets all fields to default values.
3) 3) In the Builder, create methods that mutate each of the fields
4) 4) In the builder, create a method build() that creates the object with the current values of the fields
5) In the original class, add a public [[Static Methods|Static]] method builder() that creates and returns the Builder