import processing.sound.*;

PFont font;
PShape bot;
SoundFile sound;


int a= num = 35;
//PImage flags[];
//String texts[];

String flags[] = { "W_000", "W_001", "W_002", "W_003", "W_004", "W_005", "W_006", "W_007", "W_008", "W_009", "W_010", 
"W_011", "W_012", "W_013", "W_014","W_015","W_016","W_017","W_018","W_019","W_020","W_021","W_022","W_023","W_024","W_025"
,"W_026","W_027","W_028","W_029","W_030","W_031","W_032","W_033","W_034","W_035","W_036","W_037","W_038","W_039","W_040"};
String texts[] = { "T_000", "T_001", "T_002", "T_003", "T_004", "T_005", "T_006", "T_007", "T_008", "T_009", "T_010", "T_011", "T_012", "T_013", "T_014"
, "T_015", "T_016", "T_017", "T_018", "T_019", "T_020", "T_021", "T_022", "T_023", "T_024", "T_025", "T_026", "T_027", "T_028", "T_029"
, "T_030", "T_031", "T_032", "T_033", "T_034", "T_035", "T_036", "T_037", "T_038", "T_039", "T_040"};
PImage flagImage;
String name = "";
String nature = "";
String str = "";
int index = 0;

import controlP5.*;
ControlP5 cp5;

Textarea nameText;
Textarea historyText;
Textarea natureText;
Textarea politicsText;
Textarea diplomacyText;
Textarea economyText;
Textarea societyText;
Textarea cultureText;
Textarea time_differenceText;
Textarea colonyText;

String str_nameText = "";
String str_historyText = "";
String str_natureText = "";
String str_politicsText = "";
String str_diplomacyText = "";
String str_economyText = "";
String str_societyText = "";
String str_cultureText = "";
String str_time_differenceText = "";
String str_colonyText = "";

String moving_str_nameText = "";
String moving_str_historyText = "";
String moving_str_natureText = "";
String moving_str_politicsText = "";
String moving_str_diplomacyText = "";
String moving_str_economyText = "";
String moving_str_societyText = "";
String moving_str_cultureText = "";
String moving_str_time_differenceText = "";
String moving_str_colonyText = "";

int id = 0;

int cnt = 0;

void setup() {
  size(2600, 1500);
   balls = new Ball [ num ];
  for ( int i = 0; i < num; i++ ) {
    balls[i] = new Ball( i ); //
  }
  //bot = loadShape("ADD_003.svg");
  sound = new SoundFile(this, "music_000.mp3");
  sound.play();
  //flags = new PImage [14];
  //texts = new String [14];

  //for ( int i = 0; i < flags.length; i++ ) {
  //String file_name = "W_" + nf(i, 3, 0 ) + ".png";
  //flags[i] = loadImage("W_" + nf(i, 3, 0 ) + ".png");
  //}

  //for ( int i = 0; i < texts.length; i++ ) {
  //String file_name = "T_" + nf(i, 3, 0 ) + ".txt";
  //texts[i] = loadStrings("T_" + nf(i, 3, 0 ) + ".txt");
  //}


  cp5 = new ControlP5(this);

  nameText = cp5.addTextarea("nameText")
    .setPosition(1000, 100)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  nameText.setText("");

  historyText = cp5.addTextarea("historyText")
    .setPosition(1000, 200)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  historyText.setText("");

  natureText = cp5.addTextarea("natureText")
    .setPosition(1000, 510)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  natureText.setText("");

  politicsText = cp5.addTextarea("politicsText")
    .setPosition(1000, 700)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  politicsText.setText("");

  diplomacyText = cp5.addTextarea("diplomacyText")
    .setPosition(1000, 800)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  diplomacyText.setText("");

  economyText = cp5.addTextarea("economyText")
    .setPosition(1000, 900)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  economyText.setText("");

  societyText = cp5.addTextarea("societyText")
    .setPosition(1000, 1050)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  societyText.setText("");

  cultureText = cp5.addTextarea("cultureText")
    .setPosition(1000, 1150)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  cultureText.setText("");

  time_differenceText = cp5.addTextarea("time_differenceText")
    .setPosition(1000, 1250)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  time_differenceText.setText("");

  colonyText = cp5.addTextarea("colonyText")
    .setPosition(1000, 1320)
    .setSize(1400, 500)
    .setFont(createFont("HBIOS-SYS.ttf", 30))
    .setLineHeight(33)
    .setColor(color(#00FCFA))
    //.setColorBackground(color(0))
    .setColorForeground(color(255, 100));
  ;
  colonyText.setText("");

  printArray ( font.list() );
  font = createFont( font.list()[460], 30 );
  textFont(font);
}


void draw() {
  background(0);
  fill(0);
  rect(0, 0, width, height);
  
  beginShape();
  for ( int i = 0; i < num - 1; i += 2 ) {
    Ball b = balls[ i ];
    Ball nb = balls[ i+1 ];
    stroke(#39FFFD);
    curveVertex( b.posX, b.posY );
    curveVertex( nb.posX, nb.posY );
  }

  endShape();

  for ( int i = 0; i < num; i ++ ) {
    balls[i].update();
    //balls[i].display();
  }

  //shape(bot, -809, -285, 2655, 1750);

  if ( flagImage != null )
    image(flagImage, 210, 350);

  if ( cnt == 0 ) {
    loadNation(id);
    id = id + 1;
    if ( id == flags.length ) {
      id = 0;
    }
  }
  cnt ++;


  if ( cnt > 900 ) { //300 프레임(5초) 마다 리셋
    cnt = 0;
  }

  float main_progress = (float) cnt / 800; // 0.0 ~ 1.0 : 200 동안 0에서 1로 증가

  float progress_name = constrain( map(main_progress, 0, 0.1, 0, 1), 0, 1 ); // main_progress 0 ~ 0.1 동안 진행
  float progress_history = constrain( map(main_progress, 0.1, 0.2, 0, 1), 0, 1 ); // main_progress 0.1 ~ 0.2 동안 진행
  float progress_nature = constrain( map(main_progress, 0.2, 0.3, 0, 1), 0, 1 );
  float progress_politics = constrain( map(main_progress, 0.3, 0.4, 0, 1), 0, 1 );
  float progress_diplomacy = constrain( map(main_progress, 0.4, 0.5, 0, 1), 0, 1 );
  float progress_economy = constrain( map(main_progress, 0.5, 0.6, 0, 1), 0, 1 );
  float progress_society = constrain( map(main_progress, 0.6, 0.7, 0, 1), 0, 1 );
  float progress_culture = constrain( map(main_progress, 0.7, 0.8, 0, 1), 0, 1 );
  float progress_time = constrain( map(main_progress, 0.8, 0.9, 0, 1), 0, 1 );
  float progress_colony = constrain( map(main_progress, 0.9, 0.99, 0, 1), 0, 1 );


  moving_str_nameText = str_nameText.substring(0, int( progress_name * str_nameText.length() ) );
  moving_str_historyText = str_historyText.substring(0, int( progress_history * str_historyText.length() ) );
  moving_str_natureText = str_natureText.substring(0, int( progress_nature * str_natureText.length() ) );
  moving_str_politicsText = str_politicsText.substring(0, int( progress_politics * str_politicsText.length() ) );
  moving_str_diplomacyText = str_diplomacyText.substring(0, int( progress_diplomacy * str_diplomacyText.length() ) );
  moving_str_economyText = str_economyText.substring(0, int( progress_economy * str_economyText.length() ) );
  moving_str_societyText = str_societyText.substring(0, int( progress_society * str_societyText.length() ) );
  moving_str_cultureText = str_cultureText.substring(0, int( progress_culture * str_cultureText.length() ) );
  moving_str_time_differenceText = str_time_differenceText.substring(0, int( progress_time * str_time_differenceText.length() ) );
  moving_str_colonyText = str_colonyText.substring(0, int( progress_colony * str_colonyText.length() ) );


  nameText.setText(moving_str_nameText);
  historyText.setText(moving_str_historyText);
  natureText.setText(moving_str_natureText);
  politicsText.setText(moving_str_politicsText);
  diplomacyText.setText(moving_str_diplomacyText);
  economyText.setText(moving_str_economyText);
  societyText.setText(moving_str_societyText);
  cultureText.setText(moving_str_cultureText);
  time_differenceText.setText(moving_str_time_differenceText);
  colonyText.setText(moving_str_colonyText);
  
  saveFrame("mov/####.tif");

}

void loadNation( int id ) {
  flagImage = loadImage ( flags[id]+ ".png" );
  String[] lines = loadStrings(  texts[id]+ ".txt" );
  println(lines.length); // 11줄인 경우가 있습니다. 체크 필요! 

  str_nameText = lines[0];
  str_historyText = lines[1];
  str_natureText = lines[2];
  str_politicsText = lines[3];
  str_diplomacyText = lines[4];
  str_economyText = lines[5];
  str_societyText = lines[6];
  str_cultureText = lines[7];
  str_time_differenceText = lines[8];
  str_colonyText = lines[9];

}


Ball balls[];
int num = 29;{
  balls = new Ball [ num ];
  for ( int i = 0; i < num; i++ ) {
    balls[i] = new Ball( i ); //
  }
}
  
  
  

class Ball {
  int id; //
  float posX, posY, speedX, speedY, size;
  color c;
  Ball( int _id ) { //
    id = _id; //
    posX = random(width);
    posY = random(height);
    speedX = random(-5, 7);
    speedY = random(-5, 7);
    size = random(90, 30);
    c = color( random(255), random(120), random(255) );
  }
  void update() {

    posX = posX + speedX;
    posY = posY + speedY;
    if ( posX < 0 || posX > width ) {
      speedX *= -1;
      c = color( random(255), random(120), random(255) );
    }
    if ( posY < 0 || posY > height ) {
      speedY *= -1;
      c = color( random(255), random(120), random(255) );
    }
  }
  void display() {
    fill(c, 100);
    noStroke();
    ellipse( posX, posY, size, size );
    fill(255);
    text(id, posX-2, posY+3);
  }
}
