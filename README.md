from OpenGL.GL import *
from OpenGL.GLUT import *
import numpy as np
from math import *

def circle(r=.25,xc=0,yc=0):
    glBegin(GL_POLYGON)

    for theta in np.arange(0,2*pi,.001):
        x=r*cos(theta)
        y=r*sin(theta)
        glVertex(x+xc,y+yc)
      

    glEnd()


def draw():
    glClearColor(1,1,1,1)
    glClear(GL_COLOR_BUFFER_BIT)
    glColor3f(1,0,0)

    glBegin(GL_POLYGON)
    glColor3f(.2,0,.1)
    glVertex(-.45,-.5)
    glVertex(-.45,-.55)
    glVertex(-.25,-.55)
    glVertex(-.25,-.4)
    glVertex(-.3,-.4)
    glVertex(-.3,-.5)
    glVertex(-.45,-.5)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.2,0,.1)
    glVertex(.45,-.5)
    glVertex(.45,-.55)
    glVertex(.25,-.55)
    glVertex(.25,-.4)
    glVertex(.3,-.4)
    glVertex(.3,-.5)
    glVertex(.45,-.5)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.9,.8,.3)
    glVertex(.4,.5)
    glVertex(-.4,.5)
    glVertex(-.4,-.5)
    glVertex(.4,-.5)
    glEnd()

    glBegin(GL_LINE_LOOP)
    glColor3f(.2,0,.1)
    glVertex(.4,.5)
    glVertex(-.4,.5)
    glVertex(-.4,-.5)
    glVertex(.4,-.5)
    glEnd()
    
    glBegin(GL_QUADS)
    glColor3f(.9,.8,.5)
    glVertex(-.1,.5)
    glVertex(.1,.5)
    glVertex(.1,.7)
    glVertex(-.1,.7)
    glEnd()
    
    glBegin(GL_LINE_LOOP)
    glColor3f(.2,0,.1)
    glVertex(-.1,.5)
    glVertex(.1,.5)
    glVertex(.1,.7)
    glVertex(-.1,.7)
    glEnd()

    glBegin(GL_QUADS)
    glColor3f(.9,.8,.5)
    glVertex(-.05,.7)
    glVertex(.05,.7)
    glVertex(.05,.9)
    glVertex(-.05,.9)
    glEnd()

    glBegin(GL_LINE_LOOP)
    glColor3f(.2,0,.1)
    glVertex(-.05,.7)
    glVertex(.05,.7)
    glVertex(.05,.9)
    glVertex(-.05,.9)
    glEnd()
    
    glBegin(GL_POLYGON)
    glColor3f(.2,.6,.9)
    glVertex(.02,.96)
    glVertex(.1,.97)
    glVertex(.19,.96)
    glVertex(.19,.84 )
    glVertex(.1,.83)
    glVertex(.02,.84)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.2,.6,.9)
    glVertex(-.18,.96)
    glVertex(-.1,.97)
    glVertex(-.02,.96)
    glVertex(-.02,.84 )
    glVertex(-.1,.83)
    glVertex(-.18,.84)
    glEnd()
    
    glBegin(GL_POLYGON)
    glColor3f(.5,.6,.7)
    glVertex(.45,-.3)
    glVertex(.65,-.3)
    glVertex(.65,-.7)
    glVertex(.45,-.7)
    glEnd()

    for i in np.arange(-.3,-.7,-.09):
        glBegin(GL_LINES)
        glColor3f(.2,0,.1)
        glVertex(.45,i)
        glVertex(.65,i)
        glEnd()


        
    glBegin(GL_POLYGON)
    glColor3f(.5,.6,.7)
    glVertex(-.45,-.3)
    glVertex(-.65,-.3)
    glVertex(-.65,-.7)
    glVertex(-.45,-.7)
    glEnd()

   

    for i in np.arange(-.3,-.7,-.09):
        glBegin(GL_LINES)
        glColor3f(.2,0,.1)
        glVertex(-.45,i)
        glVertex(-.65,i)
        glEnd()

    glBegin(GL_LINES)
    glColor3f(.2,0,.1)
    glVertex(-.8,-.7)
    glVertex(.8,-.7)
    glEnd()
    
    glBegin(GL_LINES)
    glColor3f(.2,0,.1)
    glVertex(-.6,-.8)
    glVertex(-.2,-.8)
    glEnd()
    
    glBegin(GL_LINES)
    glColor3f(.2,0,.1)
    glVertex(.2,-.8)
    glVertex(.6,-.8)
    glEnd()

    glBegin(GL_LINES)
    glColor3f(.2,0,.1)
    glVertex(-.2,-.9)
    glVertex(.2,-.9)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(.3,0)
    glVertex(.6,0)
    glVertex(.6,-.1)
    glVertex(.3,-.1)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(.45,0.1)
    glVertex(.55,0.1)
    glVertex(.55,-.1)
    glVertex(.45,-.1)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(.3,.2)
    glVertex(.6,.2)
    glVertex(.6,.1)
    glVertex(.3,.1)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(.4,0.07)
    glVertex(.5,0.07)
    glVertex(.5,0.05 )
    glVertex(.4,0.05)
    glEnd()


    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(-.3,0)
    glVertex(-.6,0)
    glVertex(-.6,-.1)
    glVertex(-.3,-.1)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(-.45,0.1)
    glVertex(-.55,0.1)
    glVertex(-.55,-.1)
    glVertex(-.45,-.1)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(-.3,.2)
    glVertex(-.6,.2)
    glVertex(-.6,.1)
    glVertex(-.3,.1)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.6,.6,1)
    glVertex(-.4,0.07)
    glVertex(-.5,0.07)
    glVertex(-.5,0.05 )
    glVertex(-.4,0.05)
    glEnd()

    glBegin(GL_POLYGON)
    glColor3f(.55,1,.9)
    glVertex(-.2,.35)
    glVertex(-.1,.35)
    glVertex(-.1,.45 )
    glVertex(-.2,.45)
    glEnd()

    

   


    
    
    glColor3f(.2,0,.6)
    circle(.06,.1,.9)
    glColor3f(.2,0,.6)
    circle(.06,-.1,.9)
    glColor3f(.9,1,1)
    circle(.02,.1,.9)
    glColor3f(.9,1,1)
    circle(.02,-.1,.9)
    glColor3f(1,0,.1)
    circle(.03,.1,.4)


    glFlush()



glutInit()
glutInitDisplayMode(GLUT_SINGLE | GLUT_RGB)
glutInitWindowSize(500,500)
glutCreateWindow(b"WALLE")
glutDisplayFunc(draw)
glutMainLoop()



    

