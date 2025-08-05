
// Classes and object - OOP - Object Oriented Programming
// Core Concepts
// Good For Learning Example
// Make Sure You Have Node js installed
// Run command - node index.js


class Dressup {
    constructor(name) {
        this.name = name;
        this.study = "School";
        this.class = 10;
        this.cry = true;
        this.loveFashion = true;
    }
}


class girl extends Dressup {
    constructor(name) {
        super(name)
        this.mature = false;
    }

    love() {
        return "I love you gojo!";
    }
}


class boy extends Dressup {
    constructor(name) {
        super(name)
        this.mature = true;
    }

    love() {
        return "But Iam shy";
    }
}


let Marin = new girl("Marin Kitagawa");
let Gojo = new boy("Gojo Wakana");
console.log(Marin.name, Gojo.name);
console.log(`Hi, Iam ${Marin.name}, Iam In Class ${Marin.class}`);
console.log(`hi, Iam ${Gojo.name}, Iam a ${Gojo.study} Boy`);
// Look! this.cry not used
console.log(`We are both love Fashion, it's ${Marin.loveFashion}`); // You Can Also Use ${Gojo.loveFashion}

// There are some love tease chemistry so if you are not open minded then, go away...!
console.log(Marin.love());
console.log(Gojo.love());

