# module.exports-II

module.exports II
We can also wrap any collection of data and functions in an object, and export the object using module.exports. In menu.js, we could write:

module.exports = {
  specialty: "Roasted Beet Burger with Mint Sauce",
  getSpecialty: function() {
    return this.specialty;
  } 
}; 
In the above code, notice:

module.exports exposes the current module as an object.
specialty and getSpecialty are properties on the object.
Then in order.js, we write:

const Menu = require('./menu.js');
 
console.log(Menu.getSpecialty());
