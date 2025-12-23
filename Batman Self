
#include "iGraphics.h"

int x = 100;
int y = 100;
double ax[5] = { 225, 210, 300, 390, 375 };
double ay[5] = { 210, 120, 80, 120, 210 };
double bx[4] = { 220, 225, 375, 380 };
double by[4] = { 275, 210, 210, 275 };
double cx[7] = { 300, 237, 245, 285, 315, 355, 363 };
double cy[7] = { 185, 211, 125, 110, 110, 125, 211 };
double dx[3] = { 250, 285, 259 };
double dy[3] = { 276, 266, 258 };
double ex[3] = { 350, 331, 315 };
double ey[3] = { 276, 258, 266 };
double fx[3] = { 220, 233, 240 };
double fy[3] = { 290, 370, 315 };
double gx[3] = { 367, 380, 360 };
double gy[3] = { 370, 290, 315 };
void iDraw()
{
	iClear();
	iSetColor(255, 255, 255);
	iFilledRectangle(0, 0, 600, 400);
	iSetColor(0, 0, 0);
	iFilledPolygon(ax, ay, 5);
	iSetColor(0, 0, 0);
	iFilledPolygon(bx, by, 4);
	iSetColor(0, 0, 0);
	iFilledEllipse(300, 275, 83, 60);
	iSetColor(255, 250, 204);
	iFilledPolygon(cx, cy, 7);
	iSetColor(255, 255, 255);
	iFilledPolygon(dx, dy, 3);
	iFilledPolygon(ex, ey, 3);
	iSetColor(0, 0, 0);

	iFilledPolygon(fx, fy, 3);
	iFilledPolygon(gx, gy, 3);
}


void iMouseMove(int mx, int my)
{

}

void iPassiveMouseMove(int mx, int my)
{

}

void iMouse(int button, int state, int mx, int my)
{

	if (button == GLUT_LEFT_BUTTON && state == GLUT_DOWN)
	{


	}


	if (button == GLUT_RIGHT_BUTTON && state == GLUT_DOWN)
	{

	}
}

// Special Keys:
// GLUT_KEY_F1, GLUT_KEY_F2, GLUT_KEY_F3, GLUT_KEY_F4, GLUT_KEY_F5, GLUT_KEY_F6, GLUT_KEY_F7, GLUT_KEY_F8, GLUT_KEY_F9, GLUT_KEY_F10, GLUT_KEY_F11, GLUT_KEY_F12, 
// GLUT_KEY_LEFT, GLUT_KEY_UP, GLUT_KEY_RIGHT, GLUT_KEY_DOWN, GLUT_KEY_PAGE UP, GLUT_KEY_PAGE DOWN, GLUT_KEY_HOME, GLUT_KEY_END, GLUT_KEY_INSERT

void fixedUpdate()
{
	if (isKeyPressed('w') || isSpecialKeyPressed(GLUT_KEY_UP))
	{
		y++;
	}
	if (isKeyPressed('a') || isSpecialKeyPressed(GLUT_KEY_LEFT))
	{
		x--;
	}
	if (isKeyPressed('s') || isSpecialKeyPressed(GLUT_KEY_DOWN))
	{
		y--;
	}
	if (isKeyPressed('d') || isSpecialKeyPressed(GLUT_KEY_RIGHT))
	{
		x++;
	}

	if (isKeyPressed(' ')) {
		// Playing the audio once
		mciSendString("play ggsong from 0", NULL, 0, NULL);
	}
}


int main()
{
	// Opening/Loading the audio files
	//mciSendString("open \"Audios//background.mp3\" alias bgsong", NULL, 0, NULL);
	//mciSendString("open \"Audios//gameover.mp3\" alias ggsong", NULL, 0, NULL);

	// Playing the background audio on repeat
	//mciSendString("play bgsong repeat", NULL, 0, NULL);

	// If the use of an audio is finished, close it to free memory
	// mciSendString("close bgsong", NULL, 0, NULL);
	// mciSendString("close ggsong", NULL, 0, NULL);

	iInitialize(600, 400, "Project Title");
	iStart();
	return 0;
}
