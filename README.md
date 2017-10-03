# NewtonMethod

function some() {
    var x0, z, eps, txt, txt1, k;
    eps = 0.001;
    x0 = 2;
    z = x0;
    var txt = " ";
    var txt1 = " ";
    var k = 1;
    
    
    
for (; k <= 10; k++) {
    var y, res , i;
    y = z - ( (Math.exp(z) + 2 * z * z - 5) / (Math.exp(z) + 4 * z) );
    var res = Math.abs(y - z);
    var i = 0;
        
    do {
        if (res > eps) {
            z = y;
        }
        txt += y. + "<br>" + res. + "<br>" + "<br>";
        i++;
    } while (i <= 0);    
        
    };
   
    
    document.getElementById("demo").innerHTML = txt;
    document.getElementById("demo1").innerHTML = txt1;
    return txt1;
};

document.write(some());
