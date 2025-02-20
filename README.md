let n = 5;
for (let i = 1; i <= n; i++) {
    let str = "* ";
    console.log(str.repeat(i));
}

Output
* 
* * 
* * * 
* * * * 
* * * * * 

*****
*   *
*   *
*   *
*****
The top and bottom sides of the square have the full amount of stars. All lines in between will only have one star in the beginning of the line and one star at the end of the line.

I use the following function:

function square(input) {
    // top line
    console.log('*'.repeat(input));
    // middle lines
    for(let i = 1; i < input - 1; i++) {
        console.log('*' + ' '.repeat(input-2) + '*');
    }
    // bottom line
    console.log('*'.repeat(input));
};

square(5);
