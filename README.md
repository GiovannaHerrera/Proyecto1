# Proyecto1

int numerodepantalla=0;
 
color c;

class Boton{
  
  int x, y; 
  color c; 
  
 Boton(){
 this.x=90; 
 this.y=180; 
 this.c=255; 
  
}

void display(){
  stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (90, 180, 190.5, 60.5);
  fill(255);
  text ("Seleccionar personaje (w)", 90.0, 180.0); 
  }
  
}


class Botonin{
  
  int x, y; 
  color c; 
  
 Botonin(){
 this.x=90; 
 this.y=180; 
 this.c=255; 
  
}

void display(){
  stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (180, 90, 190.5, 60.5);
  fill(255);
  text ("Jugar (a)", 180.0, 90.0); 
  }
  
}

class Botonon{
  
  int x, y; 
  color c; 
  
 Botonon(){
 this.x=90; 
 this.y=180; 
 this.c=255; 
  
}

void display(){
  stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
 rect (30, 280, 190.5, 60.5);
  fill(255);
  text ("Salir (s)", 30.0, 280.0); 
  }
  
}

 
class Banana{
  color c;
 
 Banana(){
   this.c=255;  
}

void display(int x_, int y_){
  
   pushMatrix();
   noStroke();
   translate(x_, y_);
   scale(-1,1);
   rotate (PI);
   fill(this.c, this.c, 0);
   bezier(600, 90,  600, 100,  90, 100,  90, 600);
   fill(0);
   fill(0,100,180);
   stroke(255);
   strokeWeight(2.1);
   ellipse(140,320,50, 50);
   ellipse(400,410,50, 50);
   ellipse(360,50,70, 70);
   ellipse(450,50,70, 70);
   fill(0);
   noStroke();
   ellipse(200, 500, 60, 60);
   ellipse(130, 470, 60, 60);
   fill(255);
   ellipse(200, 520, 20, 20);
   ellipse(130, 490, 20, 20);
   popMatrix(); 
}
}


Boton uno; 
Botonin dos; 
Botonon tres; 
Banana na; 
Ciudad ciudadin;

void setup(){ 
  size (1080,720); 
  background (0, 0, 0);
  textAlign(LEFT);
  textSize (20); 
  
  uno= new Boton();
  dos= new Botonin(); 
  tres= new Botonon(); 
  na= new Banana();

}


void draw(){
  fill(255);
  textSize (80); 
  text ("Banana Bangs", 30.0, 570.3); 
  textSize(18);
  text("Selecciona con las teclas que se te indiquen la opcion que quieras", 30.0, 670.0);
  
  textSize(20);
  
  uno.display(); 
  dos.display();
  tres.display(); 
  na.display(450,700);
 
  stroke(#24a4a5);  
  strokeWeight(3.3); 
  color(255); 
  line (580.3, 580.3, 100.0, 580.3);
  
  stroke(0); 
  arc(700, 300, 70, 70, 0.5, HALF_PI, CHORD);
  
    stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (90, 180, 190.5, 60.5);
  fill(255);
  text ("Seleccionar personaje (w)", 90.0, 180.0);
  
   stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (180, 90, 190.5, 60.5);
  fill(255);
  text ("Jugar (a)", 180.0, 90.0); 
  
   stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (30, 280, 190.5, 60.5);
  fill(255);
  text ("Salir (s)", 30.0, 280.0); 
  
  
  /*switch(numerodepantalla){
    case 0:
      pantalla1.seleccionPersonajes();
    break;
    case 1:
      pantalla2.seleccionPersonajes();
    break;
    case 2:
     
    break;
  }*/

  if (keyPressed){
  switch(key){
    case 'w': 
  stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (90, 180, 190.5, 60.5);
  fill(255);
  text ("Seleccionar personaje (w)", 90.0, 180.0);
    break;
    
    case 'a':
  stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (180, 90, 190.5, 60.5);
  fill(255);
  text ("Jugar (a)", 180.0, 90.0);
    break; 
    
    case 's':
  stroke(0,50,120);
  strokeWeight(3.3); 
  fill(0,100,180);
  rect (30, 280, 190.5, 60.5);
  fill(255);
  text ("Salir (s)", 30.0, 280.0); 
    break;
  }
  }
}
 
 //pantalla seleccion
 int d, s, m, j, n, i; 
int dx;
int x;
int v=8; 


class seleccionPersonajes {

  seleccionPersonajes() {
    
  }


  void display() {

    stroke(#ffdf00); 
    strokeWeight(4.5);
    rect(90.0, 100.0, 150.0, 150.0); 
    rect(340.0, 100.0, 150.0, 150.0); 
    rect(590.0, 100.0, 150.0, 150.0); 
    rect(840.0, 100.0, 150.0, 150.0); 
    rect(220.0, 300.0, 150.0, 150.0);//segunda linea
    rect(720.0, 300.0, 150.0, 150.0);// segunda linea 

    //textAlign(0);   
    textSize(20);
    text("Seleccionar", 380.0, 575.0);  
    rect(380.0, 580.0, 300.0, 75.0); 

    text("Jitomate Saladette", 90.0, 90.0);
    text("Ivanna Bannana", 340.0, 90.0);
    text("Manzana Monzon", 590.0, 90.0);
    text("Naranja Ja", 840.0, 90.0);
    text("DR. Mora", 220.0, 290.0);
    text("Sandia Watermelon", 720.0, 290.0);
  }

  void estado(int e_) { //botones de seleccion de pantalla 
    switch(e_) {
    case 0:
      int Saladette;
      break;

    case 1:
      int Bananna; 
      break;

    case 2:
      int Monzon;
      break;

    case 3:
      int Ja; 
      break;

    case 4:
      int Dr; 
      break;

    case 5:
      int Watermelon; 
      break;
    }
  }
}

// personajes

class Jitomate { 
  float x, y; 
  float v; 
  color c; 
  int ellipser=200, ellipsej=200; 
  float ataque; 

  //constructor 
  Jitomate() { 
    this.x=width/2; 
    this.y=height/2; 
    this.v=6; 
    this.c=255;

    Saladette= new Jitomate();
  }

  void display() {
    pushMatrix();
    fill (this.c, 0, 0);//jitomate 
    noStroke(); 
    ellipse(this.x, this.y, this.ellipser, this.ellipsej);
    fill(0);
    ellipse(this.x-50, this.y-40, this.ellipser-150, this.ellipsej-150);
    ellipse(this.x+50, this.y-40, this.ellipser-150, this.ellipsej-150);
    fill(255);
    ellipse(this.x-40, this.y-50, this.ellipser-170, this.ellipsej-170);
    ellipse(this.x+60, this.y-50, this.ellipser-170, this.ellipsej-170);
    fill (this.c, 0, 0);
    ellipse(this.x-150, this.y+40, this.ellipser-150, this.ellipsej-150);
    ellipse(this.x+150, this.y+40, this.ellipser-150, this.ellipsej-150);
    fill (this.c, 0, 0);
    ellipse(this.x-70, this.y+120, this.ellipser-150, this.ellipsej-170);
    ellipse(this.x+70, this.y+120, this.ellipser-150, this.ellipsej-170);
    fill(255);
    noStroke();
    arc(this.x, this.y, 80, 80, 0, PI+QUARTER_PI, CHORD);
    fill(0, this.c, 0);
    beginShape(TRIANGLES);
    vertex(510, 260);
    vertex(520, 295);
    vertex(530, 260);
    vertex(530, 260);
    vertex(540, 295);
    vertex(550, 260);
    vertex(550, 260);
    vertex(560, 295);
    vertex(570, 260);
    endShape();
    stroke(255);
    line(this.x, this.y, 400, 400);
    popMatrix();
  }

  void movimiento(int j_) {

    switch(j_) {
    case 0:
      this.y-=this.v;//arriba
      break;

    case 1:
      this.x+=this.v;//derecha
      break; 

    case 2: 
      this.x -=this.v;//izq
      break; 

    case 3:
      this.y +=this.v; //abajo
      break;
    }
  }

  void limites() {
    this.x= constrain (1030, 1030, 670); 
    this.y= constrain(1030, 1030, 670);
  }

  void ataque() {
    if (x>700) {
      dx+= 1;
      fill(255, 0, 0);
      ellipse(this.x, this.y, 40, 40);
    } 
    else if (x<50) {
      dx+= -1;
      fill(255, 0, 0);
      ellipse(this.x, this.y, 40, 40);
    }
  }
}


class Mora {
  float m, o; 
  float v; 
  color c; 
  int ellipsem=90, ellipseo=90; 
  float ataque2; 

  //constructor
  Mora() {
    this.m=width/2; 
    this.o=height/2; 
    this.v=6; 
    this.c=255;

    Dr= new Mora();
  }

  void display() {
    pushMatrix();
    fill(this.c, 0, 120); 
    noStroke(); 
    ellipse(this.m, this.o, this.ellipsem, this.ellipseo); 
    ellipse(this.m+50, this.o, this.ellipsem, this.ellipseo);  
    ellipse(this.m-50, this.o, this.ellipsem, this.ellipseo); 
    ellipse(this.m, this.o+50, this.ellipsem, this.ellipseo); 
    ellipse(this.m-50, this.o+50, this.ellipsem, this.ellipseo); 
    ellipse(this.m+50, this.o+50, this.ellipsem, this.ellipseo); 
    ellipse(this.m, this.o+100, this.ellipsem, this.ellipseo);
    fill(0);
    ellipse(this.m-30, this.o+20, this.ellipsem-70, this.ellipseo-70);
    ellipse(this.m+30, this.o+20, this.ellipsem-70, this.ellipseo-70);
    fill(255); 
    ellipse(this.m-25, this.o+20, this.ellipsem-80, this.ellipseo-80);
    ellipse(this.m+25, this.o+20, this.ellipsem-80, this.ellipseo-80);
    noFill();
    stroke(this.c, this.c, 0);
    strokeWeight(2);
    ellipse(this.m-35, this.o+20, this.ellipsem-50, this.ellipseo-50);
    ellipse(this.m+35, this.o+20, this.ellipsem-50, this.ellipseo-50);
    fill(255);
    stroke(255);
    strokeWeight(0.5);
    arc(this.m+10, this.o+80, 70, 70, 4, HALF_PI+PI, CHORD);
    noStroke();
    fill(this.c, 0, 120); 
    ellipse(this.m+125, this.o+50, this.ellipsem-50, this.ellipseo-50); 
    ellipse(this.m-125, this.o+50, this.ellipsem-50, this.ellipseo-50); 
    ellipse(this.m+25, this.o+180, this.ellipsem-50, this.ellipseo-50); 
    ellipse(this.m-25, this.o+180, this.ellipsem-50, this.ellipseo-50); 
    popMatrix();
     
  }

  void movimiento(int d_) {

    switch(d_) {
    case 0:
      this.o-=this.v;//arriba
      break;

    case 1:
      this.m+=this.v;//derecha
      break; 

    case 2: 
      this.m -=this.v;//izq
      break; 

    case 3:
      this.o +=this.v; //abajo
      break;
    }
  }

  void limites() {
    this.m= constrain(1030, 1030, 670);
    this.o= constrain(1030, 1030, 670);
  }

  void ataque() {
    if (x>700) {
      dx+= 1;
      fill(235, 188, 0);
      ellipse(this.m, this.o, 40, 40);
    } 
    else if (x<50) {
      dx+= -1;
      fill(255, 0, 0);
      ellipse(this.m, this.o, 40, 40);
    }
  }
}

  class Sandia {

    float s, w; 
    float v;  
    color c; 
    int ellipses=300, ellipsew=200;
    float ataque3; 

    //constructor 
    Sandia() {
      this.s=height/2; 
      this.w=width/2;
      this.v=6;
      this.c=255; 

      Watermelon= new Sandia();
    }

    void display() {
      pushMatrix();
      fill(0, this.c, 70);
      ellipse(this.s, this.w, this.ellipses, this.ellipsew);
      fill(0);
      ellipse(this.s-50, this.w-20, this.ellipses-240, this.ellipsew-140);
      ellipse(this.s+50, this.w-20, this.ellipses-240, this.ellipsew-140);
      fill(255);
      ellipse(this.s-50, this.w-40, this.ellipses-280, this.ellipsew-180);
      ellipse(this.s+50, this.w-40, this.ellipses-280, this.ellipsew-180);
      fill(255);
      arc(370, 570, 70, 70, 0.5, HALF_PI, CHORD);
      fill(0, this.c, 70);
      ellipse(this.s-140, this.w+30, this.ellipses-260, this.ellipsew-160);
      ellipse(this.s+140, this.w+30, this.ellipses-260, this.ellipsew-160);
      fill(0, this.c, 70);
      ellipse(this.s-70, this.w+120, this.ellipses-250, this.ellipsew-160);
      ellipse(this.s+70, this.w+120, this.ellipses-250, this.ellipsew-160);

      popMatrix();
    }

    void movimiento(int s_) {

      switch(s_) {
      case 0:
        this.w-=this.v;//arriba
        break;

      case 1:
        this.s+=this.v;//derecha
        break; 

      case 2: 
        this.s -=this.v;//izq
        break; 

      case 3:
        this.w +=this.v; //abajo
        break;
      }
    }

    void limites() {
      this.s= constrain(1030, 1030, 670);
      this.w= constrain(1030, 1030, 670);
    }

    void ataque() {
      if (x>700) {
        dx+= 1;
        fill(0, 255, 0);
        ellipse(this.s, this.w, 60, 40);
      } 
      else if (x<50) {
        dx+= -1;
        fill(0, 255, 0);
        ellipse(this.s, this.w, 60, 40);
      }
    }    
  }

    class Manzana {

      float mn, ma; 
      float v; 
      color c; 
      int ellipsema=200, ellipsemo=100;
      float ataque4; 

      //constructor
      Manzana() {
        this.mn=width/2;
        this.ma=height/2; 
        this.c=255;

        Monzon= new Manzana();
      }

      void display() {
        pushMatrix();
        fill(255, 0, 0);
        ellipse(this.mn, this.ma, this.ellipsema, this.ellipsemo);
        ellipse(this.mn, this.ma, 60, this.ellipsemo);
        ellipse(this.mn, this.ma, 60, this.ellipsemo);
        popMatrix();
      }

      void movimiento(int m_) {

        switch(m_) {
        case 0:
          this.ma-=this.v;//arriba
          break;

        case 1:
          this.mn+=this.v;//derecha
          break; 

        case 2: 
          this.mn-=this.v;//izq
          break; 

        case 3:
          this.ma+=this.v; //abajo
          break;
        }
      }

      void limites() {
        this.mn= constrain(1030, 1030, 670);
        this.ma= constrain(1030, 1030, 670);
      }

      void ataque() {
        if (x>700) {
          dx+= 1;
          fill(255, 0, 0);
          rect(this.mn, this.ma, 40, 40);
        } 
        else if (x<50) {
          dx+= -1;
          fill(255, 0, 0);
          rect(this.mn, this.ma, 40, 40);
        }
      }
    }

      class Naranja {
        float a, t; 
        float v; 
        color c; 
        int ellipsea=180, ellipset=180; 
        float ataque5; 

        //constructor;
        Naranja() {
          this.a=300; 
          this.t=200; 
          this.v=6; 
          this.c= 255; 

          Ja= new Naranja();
        }

        void display() {
          pushMatrix();
          fill(this.c, 120, 0); 
          noStroke();
          ellipse(this.a, this.t, this.ellipsea, this.ellipset);
          fill(this.c, this.c, 0); 
          ellipse(this.a+10, this.t-70, this.ellipsea-160, this.ellipset-170);
          ellipse(this.a-50, this.t-60, this.ellipsea-160, this.ellipset-170);
          ellipse(this.a-20, this.t-40, this.ellipsea-160, this.ellipset-170);
          ellipse(this.a-30, this.t-70, this.ellipsea-160, this.ellipset-170);
          ellipse(this.a-10, this.t-60, this.ellipsea-160, this.ellipset-170);
          fill(0);
          ellipse(this.a-50, this.t+10, this.ellipsea-140, this.ellipset-140);
          ellipse(this.a+50, this.t+10, this.ellipsea-140, this.ellipset-140);
          fill(255);
          ellipse(this.a-50, this.t, this.ellipsea-160, this.ellipset-160);
          ellipse(this.a+50, this.t, this.ellipsea-160, this.ellipset-160);
          stroke(0);
          strokeWeight(0.5);
          fill(0);
          arc(290, 270, 70, 70, 4, HALF_PI+PI, CHORD);
          fill(this.c, 120, 0); 
          ellipse(this.a-120, this.t+25, this.ellipsea-150, this.ellipset-150);
          ellipse(this.a+120, this.t+25, this.ellipsea-150, this.ellipset-150);
          ellipse(this.a-60, this.t+100, this.ellipsea-140, this.ellipset-150);
          ellipse(this.a+60, this.t+100, this.ellipsea-140, this.ellipset-150);
          popMatrix();
        }

        void movimiento(int n_) {

          switch(n_) {
          case 0:
            this.t-=this.v;//arriba
            break;

          case 1:
            this.a+=this.v;//derecha
            break; 

          case 2: 
            this.a -=this.v;//izq
            break; 

          case 3:
            this.t +=this.v; //abajo
            break;
          }
        }

        void limites() { 

          a= constrain(1030, 1030, 670);
          t= constrain(1030, 1030, 670);
        }

        void ataque() {
          if (x>700) {
            dx+= 1;
            fill(225, 178, 0);
            ellipse(this.a, this.t, 20, 40);
          } 
          else if (x<50) {
            dx+= -1;
            fill(255, 0, 0);
            ellipse(this.a, this.t, 20, 40);
          }
        }
      }

        class Ivanna {
          color c;
          float x_;
          float y_;
          float v; 
          float ataque6; 

          //constructor; 
          Ivanna() {
            this.c=255;

          Bananna= new Ivanna();
          }

          void display() {

            pushMatrix();
            noStroke();
            translate(x_, y_);
            scale(-1, 1);
            rotate (PI);
            fill(this.c, this.c, 0);
            bezier(600, 90, 600, 100, 90, 100, 90, 600);
            fill(0);
            fill(0, 100, 180);
            stroke(255);
            strokeWeight(2.1);
            ellipse(140, 320, 50, 50);
            ellipse(400, 410, 50, 50);
            ellipse(360, 50, 70, 70);
            ellipse(450, 50, 70, 70);
            fill(0);
            noStroke();
            ellipse(200, 500, 60, 60);
            ellipse(130, 470, 60, 60);
            fill(255);
            ellipse(200, 520, 20, 20);
            ellipse(130, 490, 20, 20);
            popMatrix();
          }

          void movimiento(int i_) {

            switch(i_) {
            case 0:
              this.y_-=this.v;//arriba
              break;

            case 1:
              this.x_+=this.v;//derecha
              break; 

            case 2: 
              this.x_ -=this.v;//izq
              break; 

            case 3:
              this.y_+=this.v; //abajo
              break;
            }
          }

          void limites() { 

            x_= constrain(1030, 1030, 670);
            y_= constrain(1030, 1030, 670);
          }

          void ataque() {
            if (x>700) {
              dx+= 1;
              fill(255, 255, 0);
              arc(this.x_, this.y_, HALF_PI,40, 40, 40);
            } 
            else if (x<50) {
              dx+= -1;
              fill(255, 255, 0);
              arc(this.x_, this.y_, HALF_PI, 40, 40, 40);
            }
          }
        }


          Jitomate Saladette; 
          Mora Dr; 
          Sandia Watermelon; 
          Manzana Monzon; 
          Naranja Ja;
          Ivanna Bananna; 

          float x_, y_;

          void Personajines() {

            if (keyPressed) {// botones de seleccion de pantalla 
              switch(key) {
              case 0:
                Saladette.movimiento(0);
                break;

              case 1:
                Bananna.movimiento(1);
                break;

              case 2:
                Monzon.movimiento(2);
                break;

              case 3:
                Ja.movimiento(3);
                break;

              case 4:
                Dr.movimiento(4); 
                break;

              case 5:
                Watermelon.movimiento(5);
                ; 
                break;
              }
            }
            background(0, 0, 0); 
            Saladette.display(); 
            Saladette.limites();
            Dr.display();
            Dr.limites();
            Watermelon.display();
            Watermelon.limites();
            Monzon.display(); 
            Monzon.limites();
            Ja.display();
            Ja.limites();
            Bananna.display();
            Bananna.limites();



            if (keyPressed) {
              switch(key) {

              case 'w': 
                Saladette.movimiento(0); 
                Dr.movimiento(0);
                Watermelon.movimiento(0);
                Monzon.movimiento(0); 
                Ja.movimiento(0);
                Bananna.movimiento(0);
                break; 

              case 'a': 
                Saladette.movimiento(1); 
                Dr.movimiento(1);
                Watermelon.movimiento(1);
                Monzon.movimiento(1); 
                Ja.movimiento(1);
                Bananna.movimiento(1);
                break; 

              case 's': 
                Saladette.movimiento(2); 
                Dr.movimiento(2);
                Watermelon.movimiento(2);
                Monzon.movimiento(2); 
                Ja.movimiento(2);
                Bananna.movimiento(2);
                break; 

              case 'd': 
                Saladette.movimiento(3); 
                Dr.movimiento(3);
                Watermelon.movimiento(3);
                Monzon.movimiento(3); 
                Ja.movimiento(3);
                Bananna.movimiento(3);
                break;
              }
            }
            
          }
    
//pantalla batalla
float dp;
 float dt;
 float x1;
 float y1;
 float l1;
 float a1;
 
int[] jugador1=new int[4];
int[] jugador2=new int[4];
int turno=0;
 
 void batalla(){
   int batalla=0;
 }

class Barra {
  float x1; 
  float y1; 
  color c; 
  int l1=170, a1=30;

  //atributos
  Barra () {//si
    this.x1=80;
    this.y1=50;
    this.c=255; 

    fill(0, this.c, 0);
    stroke(0); 
    strokeWeight(3.3);
    rect(this.x1, this.y1, this.l1, this.a1); 
    fill(255);
    text("Dr. Mora", this.x1, this.y1);
  }
}

class Ciudad {//si

  Barra vida;
  float dt;

  Ciudad() {//si
    vida= new Barra();
     ciudadin= new Ciudad();
  }
}  


void Ciudadela() {//si
  textSize(28);
  text("Muevete con w (arriba),s(izquierda), a(derecha), d(abajo) y esquiva los ataques", 30.0, 570.0); 

  dt+=0.01;
  background(0);
  noStroke();
  for (int i= 0; i<width; i+=10) {//si
    for (int j = 0; j<height; j+=10) {//si
      fill(noise(i*0.01+dt*1, j*0.01+1, dt)*255, noise(i*0.01+dt*2, j*0.01*2, dt)*255);
      noStroke();
      rect(i, j, i, j);
    }
  }

  fill(0); //contorno de la ciudad 
  stroke(255);
  strokeWeight(5.5);
  rect(15.0, 200.0, 300.0, 600.0);
  rect(320.0, 100.0, 200.0, 700.0);
  rect(520.0, 300.0, 240.0, 500.0);
  rect(760.0, 100.0, 200.0, 700.0);
  rect(960.0, 200.0, 100.0, 600.0);

  fill(240, 225, 0);
  stroke(255);
  strokeWeight(1);
  rect(45.0, 250.0, 60.0, 60.0); //primer edificio
  rect(220.0, 250.0, 60.0, 60.0); 
  rect(45.0, 380.0, 60.0, 60.0);
  rect(220.0, 380.0, 60.0, 60.0); 
  rect(45.0, 510.0, 60.0, 60.0);
  rect(220.0, 510.0, 60.0, 60.0); 
  fill(0, 180, 255);
  rect(100.0, 630.0, 120.0, 200.0);


  fill(0, 180, 255);// segundo edificio
  stroke(255);
  noStroke();
  ellipse(370.0, 180.0, 60.0, 100.0);
  ellipse(470.0, 180.0, 60.0, 100.0);
  ellipse(370.0, 290.0, 60.0, 100.0);
  ellipse(470.0, 290.0, 60.0, 100.0);
  ellipse(370.0, 400.0, 60.0, 100.0);
  ellipse(470.0, 400.0, 60.0, 100.0);
  ellipse(370.0, 510.0, 60.0, 100.0);
  ellipse(470.0, 510.0, 60.0, 100.0);
  ellipse(420.0, 230.0, 30.0, 30.0);
  ellipse(420.0, 330.0, 30.0, 30.0);
  ellipse(420.0, 440.0, 30.0, 30.0);
  ellipse(420.0, 550.0, 30.0, 30.0);

  fill(240, 225, 0);
  stroke(255);
  strokeWeight(2.0);
  ellipse(420.0, 680.0, 100.0, 160.0); 

  fill(180, 0, 50);// tercer edificio
  stroke(255);
  noStroke();
  arc(585, 360, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(690, 360, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(585, 430, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(690, 430, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(585, 500, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(690, 500, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(585, 570, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  arc(690, 570, 70, 70, 0.5, PI+QUARTER_PI, CHORD);
  stroke(255);
  strokeWeight(1);
  rect(605.0, 630.0, 60.0, 200.0);

  fill(200, 162, 200);// cuarto edificio
  stroke(255);
  rect(780.0, 120.0, 40.0, 90.0);
  rect(840.0, 180.0, 40.0, 90.0);
  rect(900.0, 240.0, 40.0, 90.0);
  rect(780.0, 300.0, 40.0, 90.0);
  rect(840.0, 360.0, 40.0, 90.0);
  rect(900.0, 420.0, 40.0, 90.0);
  rect(780.0, 480.0, 40.0, 90.0);
  rect(840.0, 540.0, 40.0, 90.0);
  rect(900.0, 600.0, 40.0, 90.0);
  fill(180, 0, 50);
  rect(764.0, 670.0, 90.0, 70.0);

  fill(255, 90, 0);// quinto edificio
  stroke(255);
  noStroke();
  ellipse(1010.0, 260.0, 60.0, 60.0);
  ellipse(1010.0, 340.0, 60.0, 60.0);
  ellipse(1010.0, 420.0, 60.0, 60.0);
  ellipse(1010.0, 500.0, 60.0, 60.0);
  ellipse(1010.0, 580.0, 60.0, 60.0);
  fill(190, 90, 0);
  rect(971.0, 630.0, 80.0, 200.0);

  pushMatrix();
  fill(240);
  scale(0.5);
  ellipse(1270, 290, 450, 450);
  popMatrix();

  for (int h=0; h<=170; h++) {//si
    if (dp>170) {//si
      rect(this.x1, this.y1, this.l1-34, this.a1);
}

for (int f=0; f<=-170; f++) {//si
  if (dp>-170) {//si
    rect(this.x1, this.y1, this.l1+34, this.a1);
    
  
  }
}
}
}

//pantalla final
void fin(){
  int fin=0;
}
float h=170;

class Opcion{ //boton uno 
  float x;
  float y; 
  color c; 
  int l=170, a=80; 
  
  //atributos
  
  Opcion(){
  this.x=220; 
  this.y=530; 
  this.c=255; 
  unopuntouno= new Opcion();
  }

   
void Opcion1(){
  if(keyPressed){
    switch(key){
    case 0:
   fill(0, this.c, this.c); 
   stroke(255);
   strokeWeight(2);
   rect( this.x, this.y, l, a); 
   fill(255);
   textSize(28);
   text("Inicio",220, 527);
   break;
    }
}
   
}
}

class Letras{
  float x;
  float y; 
  color c; 
  
  //atributos
  
  Letras(){
  this.x=540; 
  this.y=360; 
  this.c=255;
  
  leibles= new Letras();
  
}
void Display(){
  
   fill(this.c, this.c,0); 
   noStroke();
   textSize(100);
   textAlign(CENTER);
   
   if(jugador1[2]<=0){
   text("GANASTE J1", this.x, this.y);
   }
   if (jugador1[2] <= 0)
      {
        jugador1[2]=0;
      }
   
    else if (jugador2[2]<=0){
     text("GANASTE J2", this.x, this.y);
}
if (jugador2[2] <= 0)
      {
        jugador2[2]=0;
      }  
    stroke(255,255,0);
  line (1010.0, 400.3, 80.0, 400.3);

}
}
  

Letras leibles; 
Opcion unopuntouno; 
Opcion2 dospuntodos; 


class Opcion2{ //boton uno 
  float x;
  float y; 
  color c; 
  int l=170, a=80; 
  
  //atributos
  
  Opcion2(){
  this.x=650; 
  this.y=530; 
  this.c=255; 
  dospuntodos= new Opcion2(); 
  }
   
  }
    
void Opcion22(){
   if(keyPressed){
     switch(key){
       case 1:
   fill(0, this.c, this.c); 
   stroke(255);
   strokeWeight(2);
   rect( 650,530,170,80); 
   fill(255);
   textSize(28);
   text("Salir",650, 527);
   break;
     }
   }
  
  leibles.Display();
  
}

