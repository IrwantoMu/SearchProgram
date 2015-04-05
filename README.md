# SearchProgram
first stage search program
var text = "Irwanto is an undergraduate from \
UNPAD law faculty. He spent seven years to completed the \
courses. Now Irwanto learning how to code.";
var myName = "Irwanto";
var hits = [];
for (var i = 0; i < text.length; i++) {
    if (text[i] === "I") {
        for (var j = i; j < (myName.length + i); j++) {
            hits.push(text[j]);
        }
    }
};
if (hits.length === 0) {
    console.log("Your name wasn't found!")
} else {
console.log(hits);
};
