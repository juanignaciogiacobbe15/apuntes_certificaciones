# Single Responsibility Principle(SRP)
- Just because you can doesn't mean you should.
- THERE SHOULD NEVER BE MORE THAN ONE REASON FOR A CLASS TO CHANGE.
- In this context, we define a responsibility to be “a reason for change.” If you can think of more than one motive for changing a class, then that class has more than one responsibility
- If a class assumes more than one responsibility, then there will be more than one reason for it to change.
- If a class has more then one responsibility, then the responsibilities become coupled. Changes to one responsibility may impair or inhibit the class’ ability to meet the others. This kind of coupling leads to fragile designs that break in unexpected ways when changed