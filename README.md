var r=255;
var g=255;
var b=255;
var r1=1;
var g1=1;
var b1=1;
function drawString()
{
var screen_size = Render.GetScreenSize();
Render.String( 10,screen_size[1]-99, 0, "                  SANT+Q839479611 QUN+908044982", [ r, g, b, 255 ],4 );
r=r-1*r1;
    g=g-2*g1;
    b=b-3*b1;
    if(r==1){r1=-r1;}
    if(g==1){g1=-g1;}
    if(b==1){b1=-b1;}
    if(r==255){r1=-r1;}
    if(g==255){g1=-g1;}
    if(b==255){b1=-b1;}
}

Cheat.RegisterCallback("Draw", "drawString")
