A #lang java-processing

So you can write Java processing code in DrRacket
  Does nothing fancy.  Just spits the editor string out into a file and invokes the java-processing command with the appropriate command-line flags

Example code:

```
int i = 0;
void setup(){
    background(0);
    size(300, 300);
}
void draw(){
    stroke(random(255), random(0), random(0), 100);
    line(i, 0, random(0, width), height);
    if(i < width){
        i = 1 + i;
    }
    else{
        i = 0;
    }
}
```
