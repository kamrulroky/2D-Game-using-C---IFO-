#include<iostream.h>
#include<conio.h>
#include<graphics.h>
#include<dos.h>
#include<process.h>
#include<stdlib.h>

#define LEFT 75
#define RIGHT 77
#define UP 72
#define DOWN 80
#define ENTER 13
#define SPACEBAR 32

//MOVING BORDER LINE
//COLRORING THE TEXTS

void UFO(int x, int y)
{
    x=x-20,y=y-20;
    int  ufo_wing[]= {30+x,50+y,20+x,25+y,35+x,30+y,40+x,25+y,45+x,30+y,60+x,25+y,49+x,50+y},
		     ufo_cockpit[]= {35+x,50+y,40+x,80+y,45+x,50+y};
    int x_axis_of_circle = 40, y_axis_of_circle = 50, radius;

    setcolor(BLACK);
    setfillstyle(1,7);
    fillpoly(7,ufo_wing);
    fillpoly(3,ufo_cockpit);

    for ( radius = 5; radius <= 11 ; radius = radius + 2)
    {
	setcolor(RED);
	circle(x_axis_of_circle+x,y_axis_of_circle+y,radius);
    }


}
void border(int i)
{
	for (int j = i;j < 70;j += 5 )
    {
	setcolor( RED );
	setfillstyle( 9, RED );
	bar( 16 * 8, j * 8, 17 * 8, ( j + 2 ) * 8 );
	bar( 63 * 8, j * 8, 64 * 8, ( j + 2 ) * 8 );
    }

}
void border_clear(int i)
{
	for (int j = i;j < 70;j += 5 )
    {
	setcolor( BLACK );
	setfillstyle( SOLID_FILL, BLACK );
	bar( 16 * 8, j * 8, 17 * 8, ( j + 2 ) * 8 );
	bar( 63 * 8, j * 8, 64 * 8, ( j + 2 ) * 8 );
    }

}





void IFO(int x, int y)
{
    x=x+20,y=y+20;
    int   points[]= {x+5,y+5,x+33,y+40,x+20,y+55,x+5,y+55,x,y+65,x-5,y+55,x-20,y+55,x-32,y+40,x-5,y+5};


    setcolor(BLACK);
    setfillstyle(1,1);

    fillellipse(x-15, y+35,3, 30);
    fillellipse(x+15, y+35,3, 30);

    fillpoly(9,points);

    fillellipse(x, y,3, 25);                       //end

}

void bullet(int a,int b)
{
    a=a+20;
    setfillstyle(1,4);
    fillellipse(a,b,2,4);

}


void IFO_clear(int x,int y)
{
    setcolor(0);
    x=x+20,y=y+20;
    int   points[]= {x+5,y+5,x+33,y+40,x+20,y+55,x+5,y+55,x,y+65,x-5,y+55,x-20,y+55,x-32,y+40,x-5,y+5};

    setfillstyle(SOLID_FILL,0);

    fillellipse(x-15, y+35,3, 30);
    fillellipse(x+15, y+35,3, 30);

    fillpoly(9,points);

    fillellipse(x, y,3, 25);
}
void bullet_clear(int a,int b)
{
    a=a+20;
    setcolor(0);
    setfillstyle(SOLID_FILL,0);
    fillellipse(a,b,2,4);
}

void UFO_clear(int x,int y)
{
    setcolor(0);
    x=x-20,y=y-20;
    int  ufo_wing[]= {30+x,50+y,20+x,25+y,35+x,30+y,40+x,25+y,45+x,30+y,60+x,25+y,49+x,50+y},
		     ufo_cockpit[]= {35+x,50+y,40+x,80+y,45+x,50+y};
    int x_axis_of_circle = 40, y_axis_of_circle = 50, radius;

    setfillstyle(SOLID_FILL,0);
    fillpoly(7,ufo_wing);
    fillpoly(3,ufo_cockpit);
    for ( radius = 5; radius <= 11 ; radius = radius + 2)
    {
	circle(x_axis_of_circle+x,y_axis_of_circle+y,radius);
    }

}

void screen_size()
{
    setcolor(BLACK);
    rectangle(137,0,504,getmaxy());                 //screen size and color
    setfillstyle(SOLID_FILL,1);
    floodfill(325,getmaxy()/2,BLACK);

}
void about()
{

	    cleardevice();
	    setcolor( 6 );
	    settextstyle( 7, 0, 4 );
	    setfillstyle( 9, 12 );
	    outtextxy( 240, 15, "ABOUT" );
	    bar( 220, 60, 370, 62 );
	    settextstyle( 2, 0, 5 );
	    setcolor( 2 );
	    outtextxy( 20, 100, "We had completed our work as a project work to our SENSEI." );
	    outtextxy( 3, 115,  "We had tried to reduce maximum problems in our program." );
	    outtextxy( 3, 130,  "Eventhough it may consist several technical and logical problems." );
	    outtextxy( 3, 165, "TASIF AND KAMRUL" );


    getch();
    return ;
}

void how_to_play()
{
    cleardevice();
    settextstyle( 7, 0, 4 );
    setcolor( 6 );
    outtextxy( 200, 10, "HOW TO PLAY" );
    textcolor( YELLOW );
    gotoxy( 3, 6 );
    cout << "\n\n\n\n\n\n\nIFO (IRRESPONSIBLE FLYING OBJECT) is a simple game in which you have to lead a\nFighter plane by avoiding and shoot ufo's on the sky.\nYou have to use the following keys to controll the IFO\n\nUP arrow key\t\t--\tForward movement\nDOWN arrow key\t\t--\tDownward movement\n<-LEFT arrow key\t--\tLeftside movement\n->RIGHT arrow key\t--\tRightside movement\nSpacebar\t\t--\tShoot bullet\nEsc key\t\t\t--\tExit from game at any time\n";
    getch();
    return ;
}

/*void logo ()
{
    for ( int i = 1;i < 250;i++ )
    {
	int p;
       //	setbkcolor(6);
	setcolor( 11 );
	setfillstyle( SOLID_FILL, LIGHTBLUE );
	settextstyle( 10, HORIZ_DIR, 3 );
	outtextxy( 100, 100, "IRRESPONSIBLE FLYING" );
	outtextxy( 240, 140, "OBJECT" );
	setcolor( 4 );
	bar3d( 50, 200, 550, 220, 10, 40 );
	setcolor( WHITE );
	settextstyle( 2, HORIZ_DIR, 5 );
	outtextxy( 290, 380, "LOADING..." );
	setfillstyle( SOLID_FILL, 24 );
	bar( 190, 400, 190 + i, 420 );
	rectangle( 190, 400, 440, 420 );
	delay( 15 );
    }
    delay( 2000 );
    cleardevice();
    return ;
} */


void GAME_PLAY()
{
      cleardevice();
      int x=300,y=350,ch,life=3,score=0,a=300,b=350,k=1; /* x is x axis of UFO,IFO and
						    UFO_clear,IFO_clear
						    y is y axis of UFO,IFO and
						    UFO_clear,IFO_clear*/
      border(k);
						    //a and b for bullets and bullets x and y axis
    char choice;                                   //choice is for restrat game (Y/N)
    screen_size();
    setcolor(WHITE);
    rectangle(550,35,635,80);
    gotoxy(70,4);
    cout<<"Press <Esc>";
    gotoxy(70,5);
    cout<<" to Exit";


    for(int level=1; (level<=5)&&(life>0); level++)    //loop for level and life check
    {
	if(level==1)
	{
	    gotoxy(1,5);
	    cout<<"LEVEL 1";
	    gotoxy(1,7);
	    cout<<"SHOOT UFO";
	    delay(500);
	    gotoxy(1,5);
	    cout<<"       ";
	    gotoxy(1,7);
	    cout<<"         ";
	}
	else
	{
	    gotoxy(1,5);
	    cout<<"Next level.";
	    delay(500);
	    gotoxy(1,5);
	    cout<<"           ";
	}
	for(int i=0; (i<15)&&(life>0); i++)        //loop for life and each levels ufo check
	{

	    if((level==5)&&(i==14))
	    {
		gotoxy(1,5);
		cout<<"You have won";
		gotoxy(1,6);
		cout<<"Wanna continue";
		gotoxy(1,7);
		cout<<"<y/n>";
		choice = getch();
		if ((choice=='y')||(choice=='Y'))
		    GAME_PLAY();
		else
		    exit(0);
	    }


	    setcolor(WHITE);
	    rectangle(550,125,635,175);
	    gotoxy(70,10);
	    cout<<"Level = "<<level;

	    int accident=0,clear=0;
	    //accident for clash of ufo and ifo
	    //clear for clear ufo's by serial
	    int shoot1=0,shoot2=0,shoot3=0,shoot4=0;      //shoot1,2,3,4 for clear ufo's after bullet clash
	    int y1=1,x1=300+((rand()%4)*50);
	    int y2=50,x2=250+((rand()%4)*50);
	    int y3=1,x3=200+((rand()%4)*50);
	    int y4=30,x4=200+((rand()%4)*50);        //x1,x2,x3,x4 for ufo1,ufo2,ufo3,ufo4 x axis and y1,y2,y3,y4 for y axis
	    // score += 20;
	    while(y1<getmaxy()-1)                    // loop for move ufo's downwards
	    {

		if(clear==0)
		{
		    UFO_clear(x1,y1);
		     y1++;
		    UFO(x1,y1);

		    UFO_clear(x2,y2);
		     y2++;
		    UFO(x2,y2);

		    if(level>=2){
		    UFO_clear(x3,y3);
		     y3++;
		    UFO(x3,y3); }

		    if(level>=4){
		    UFO_clear(x4,y4);
		    y4++;
		    UFO(x4,y4);}

	       border_clear(k);
	       border_clear(k-60);
	       k++;
	       border(k);
	       border(k-60);
	       if(k==70)
	       k=1;

		}
		if(accident == 3)
		{
		    if(clear==1)
		    {

			UFO_clear(x1,y1);
			if(shoot2==0){
			UFO_clear(x2,y2);
				y2++;UFO(x2,y2);}

		       if(level>=2)
			if(shoot3==0){
			UFO_clear(x3,y3);
				y3++;UFO(x3,y3);}

		       if(level>=4)
			if(shoot4==0){
			UFO_clear(x4,y4);
				y4++;UFO(x4,y4); }

			y1-=3;
			x1=150;

			if( (y3==getmaxy()-1) || (y4==getmaxy()-1) || (y2==getmaxy()-1) )
			    accident=2;

			if(level==1)
			if( (shoot1==1) && (shoot2==1) )
			{
			    UFO_clear(x2,y2);
			    break;
			}

			if( (level==2) || (level==3) )
			if( (shoot1==1) && (shoot2==1) && (shoot3==1) )
			{
			    UFO_clear(x2,y2);
			    UFO_clear(x3,y3);
			    break;
			}

			if(level>=4)
			if( (shoot1==1) && (shoot2==1) && (shoot3==1) && (shoot4==1) )
			{

			    UFO_clear(x2,y2);
			    UFO_clear(x3,y3);
			    UFO_clear(x4,y4);
			    break;
			}
			 border_clear(k);
	       border_clear(k-60);
	       k++;
	       border(k);
	       border(k-60);
	       if(k==70)
	       k=1;

		    }
		    if(clear==2)
		    {

			UFO_clear(x2,y2);
			if(shoot1==0){
			UFO_clear(x1,y1);
				y1++;UFO(x1,y1);}

			if(level>=2)
			if(shoot3==0){
			UFO_clear(x3,y3);
				y3++;UFO(x3,y3);}

			if(level>=4)
			if(shoot4==0){
			UFO_clear(x4,y4);
				y4++;UFO(x4,y4);}

			y2-=3;
			x2=150;

			if( (y1==getmaxy()-1) || (y3==getmaxy()-1) || (y4==getmaxy()-1) )
			    accident=2;

			if(level==1)
			if( (shoot1==1) && (shoot2==1) )
			{
			    UFO_clear(x1,y1);
			    break;
			}

			if( (level==2) || (level==3) )
			if( (shoot1==1) && (shoot2==1) && (shoot3==1) )
			{
			    UFO_clear(x1,y1);
			    UFO_clear(x3,y3);
			    break;
			}

		       if(level>=4)
		       if( (shoot1==1) && (shoot2==1) && (shoot3==1) && (shoot4==1) )
			{

			    UFO_clear(x1,y1);
			    UFO_clear(x3,y3);
			    UFO_clear(x4,y4);
			    break;

			}
			 border_clear(k);
	       border_clear(k-60);
	       k++;
	       border(k);
	       border(k-60);
	       if(k==70)
	       k=1;

		    }
		    if(clear==3)
		    {
			UFO_clear(x3,y3);
			if(shoot1==0){
			UFO_clear(x1,y1);
				y1++;UFO(x1,y1);}
			if(shoot2==0){
			UFO_clear(x2,y2);
				y2++;UFO(x2,y2);}

			if(level>=4)
			if(shoot4==0){
			UFO_clear(x4,y4);
				y4++;UFO(x4,y4);}

			y3-=3;
			x3=150;

			if(y1==getmaxy()-1 || (y2==getmaxy()-1) || (y4==getmaxy()-1) )
			   accident=2;

			if(level==2 || level==3)
			if( (shoot1==1) && (shoot2==1) && (shoot3==1) )
			{
			    UFO_clear(x1,y1);
			    UFO_clear(x2,y2);
			    break;
			}

		       if(level>=4)
		       if( (shoot1==1) && (shoot2==1) && (shoot3==1) && (shoot4==1) )
			{

			    UFO_clear(x2,y2);
			    UFO_clear(x1,y1);
			    UFO_clear(x4,y4);
			    break;


			}
			 border_clear(k);
	       border_clear(k-60);
	       k++;
	       border(k);
	       border(k-60);
	       if(k==70)
	       k=1;

		    }

		  if(clear==4)
		    {
			UFO_clear(x4,y4);
			if(shoot1==0){
			UFO_clear(x1,y1);
				y1++;UFO(x1,y1);}
			if(shoot2==0){
			UFO_clear(x2,y2);
				y2++;UFO(x2,y2);}
			if(shoot3==0){
			UFO_clear(x3,y3);
				y3++;UFO(x3,y3);}

			y4-=3;
			x4=150;

			if( (y1==getmaxy()-1) || (y2==getmaxy()-1) || (y3==getmaxy()-1) )
			   accident=2;


		     if( (shoot1==1) && (shoot2==1) && (shoot3==1) && (shoot4==1) )
			{

			    UFO_clear(x2,y2);
			    UFO_clear(x3,y3);
			    UFO_clear(x1,y1);
			    break;

			}
			 border_clear(k);
	       border_clear(k-60);
	       k++;
	       border(k);
	       border(k-60);
	       if(k==70)
	       k=1;

		    }

		}
		if(accident==2)
		{
		    UFO_clear(x1,y1);
		    UFO_clear(x2,y2);
		    if(level>=2)
		    UFO_clear(x3,y3);
		    if(level>-4)
		    UFO_clear(x4,y4);
		    break;
		}
		IFO(x,y);
		bullet(a,b);
		delay(5-level);
		if(kbhit())
		{
		    IFO(x,y);
		    ch=getch();
		    switch(ch)
		    {
		    case 27:
			exit(0);
			break;
		    case LEFT:
			IFO_clear(x,y);
			bullet_clear(a,b);
			if(x>171)
			{
			    x=x-50;
			    a=a-50;
			}
			if(x==x1)
			    if( ( ((y-y1)<50)&&((y-y1)>0) ) || ( ((y1-y)<50)&&((y1-y)>0))   )
			    {
				accident=1,clear=1,shoot1=1;
				x=x+50;
				a=a+50;
				IFO(x,y);
				goto Next1;
			    }

			if(x==x2)
			    if(( ((y-y2)<50)&&((y-y2)>0)) || ( ((y2-y)<50)&&((y2-y)>0)) )
			    {
				accident=1,clear=2,shoot2=1;
				x=x+50;
				a=a+50;
				IFO(x,y);
				goto Next1;
			    }
			if(x==x3)
			    if( ( ((y-y3)<50)&&((y-y3)>0) ) || ( ((y3-y)<50)&&((y3-y)>0))   )
			    {
				accident=1,clear=3,shoot3=1;
				x=x+50;
				a=a+50;
				IFO(x,y);
				goto Next1;
			    }
			if(x==x4)
			    if( ( ((y-y4)<50)&&((y-y4)>0) ) || ( ((y4-y)<50)&&((y4-y)>0))   )
			    {
				accident=1,clear=4,shoot4=1;
				x=x+50;
				a=a+50;
				IFO(x,y);
				goto Next1;
			    }


			IFO(x,y);
			bullet(a,b);
			break;
		    case RIGHT:
			IFO_clear(x,y);
			bullet_clear(a,b);
			if(x<420)
			{
			    x=x+50;
			    a=a+50;
			}
			if(x==x1)
			    if( ( ((y-y1)<50)&&((y-y1)>0) ) || ( ((y1-y)<50)&&((y1-y)>0))   )
			    {
				accident=1,clear=1,shoot1=1;
				x=x-50;
				a=a-50;
				IFO(x,y);
				goto Next1;
			    }

			if(x==x2)
			    if(( ((y-y2)<50)&&((y-y2)>0)) || ( ((y2-y)<50)&&((y2-y)>0)) )
			    {
				accident=1,clear=2,shoot2=1;
				x=x-50;
				a=a-50;
				IFO(x,y);
				goto Next1;
			    }
			if(x==x3)
			    if( ( ((y-y3)<50)&&((y-y3)>0) ) || ( ((y3-y)<50)&&((y3-y)>0))   )
			    {
				accident=1,clear=3,shoot3=1;
				x=x-50;
				a=a-50;
				IFO(x,y);
				goto Next1;
			    }
			if(x==x4)
			    if( ( ((y-y4)<50)&&((y-y4)>0) ) || ( ((y4-y)<50)&&((y4-y)>0))   )
			    {
				accident=1,clear=4,shoot4=1;
				x=x-50;
				a=a-50;
				IFO(x,y);
				goto Next1;
			    }

			IFO(x,y);
			bullet(a,b);
			break;
		    case UP:
			IFO_clear(x,y);
			bullet_clear(a,b);
			if(y>0)
			{
			    y=y-5;

			    b=b-5;
			}
			IFO(x,y);
			bullet(a,b);
			break;

		    case DOWN:
			IFO_clear(x,y);
			bullet_clear(a,b);
			if(y<getmaxy()-90)
			{
			    y=y+5;

			    b=b+5;
			}
			IFO(x,y);
			bullet(a,b);
			break;

		    case SPACEBAR: //bulletclear(a,b);
			for(b=350; b>0; b--)        //loop for move bullet upward
			{
			    bullet_clear(a,b);
			    bullet(a,b);

			    delay(0.9);
			    if(a==x1)
				if(b==y1)
				{
				    score+=10;
				    clear=1;
				    shoot1=1;
				    break;
				}

			    if(a==x2)
				if(b==y2)
				{
				    score+=10;
				    clear=2;
				    shoot2=1;
				    break;
				}

			     if(a==x3)
				if(b==y3)
				{
				    score+=10;
				    clear=3;
				    shoot3=1;
				    break;
				}

			     if(a==x4)
				if(b==y4)
				{
				    score+=10;
				    clear=4;
				    shoot4=1;
				    break;
				}


			}
			bullet_clear(a,b);
			b=y;


			break;
		    }
		}
		if(x==x1)
		    if(  ((y-y1)<50)&&((y-y1)>0) )
			accident=1,clear=1,shoot1=1;

		if(x==x2)
		    if(    ((y-y2)<50)&&((y-y2)>0)  )
			accident=1,clear=2,shoot2=1;

		if(x==x3)
		    if(    ((y-y3)<50)&&((y-y3)>0)  )
			accident=1,clear=3,shoot3=1;

		if(x==x4)
		    if(    ((y-y4)<50)&&((y-y4)>0)  )
			accident=1,clear=4,shoot4=1;

Next1:                                       //Next1 is for check accident and decrese life if accident occurs
		if(accident==1)
		{
		    life =life-1;

		    if(life==0)
		    {
			gotoxy(1,5);
			cout<<"GAME OVER ";
			setcolor(WHITE);
			rectangle(550,250,635,300);
			gotoxy(70,18);
			cout<<"Lives = "<<life;

			break;
		    }
		      settextstyle( 2, 0, 9 );
		      outtextxy( 180, 150, "ONE CHANCE LOST" );
		       delay( 1000 );

		}
		screen_size();
		setcolor(WHITE);
		rectangle(550,250,635,300);
		gotoxy(70,18);
		cout<<"Lives = "<<life;

		rectangle(550,350,635,400);
		gotoxy(70,24);
		cout<<"Score= "<<score;
		accident=3;
	    }
	}

    }

}

void menu()
{
    int s = 1, t = 0, a, p = 140;
    do
    {
	do
	{
	    cleardevice();
	    setcolor( YELLOW );
	    settextstyle( 1, 0, 4 );
	    outtextxy( 230, 30, "MENU" );
	    setfillstyle( 1, 11 );
	    bar( 140, 80, 400, 82 );
	    settextstyle( 1, 0, 1 );
	    setcolor( 11 );
	    outtextxy( 220, 137, "PLAY GAME" );
	    outtextxy( 220, 167, "HOW TO PLAY" );
	    outtextxy( 220, 197, "ABOUT" );
	    outtextxy( 220, 227, "EXIT" );
	    setcolor( RED );
	    rectangle( 200, p, 350, p + 20 );
	    a = getch();
	    switch ( a )
	    {
	    case UP: if ( p > 140 )
		{
		    p -= 30;
		    s--;
		}
		break;
	    case DOWN: if ( p < 230 )
		{
		    p += 30;
		    s++;
		};
		break;
	    case ENTER: a = 1;
		break;
	    default: break;
	    }
	}
	while ( a != 1 );
	switch ( s )
	{
	case 1: GAME_PLAY();
		 break;
	case 2: how_to_play();
		 break;
	case 3: about();
		break;
	case 4: exit( 0 );
		 break;
	}
    }
    while ( t == 0 );
    getch();

}



void main()
{
    int gdriver = DETECT,gmode;
    initgraph(&gdriver,&gmode,"C:\\TC\\BGI");
     cleardevice();
   // logo();
   // setbkcolor(BLACK);
     menu();

    getch();
    closegraph();
}
