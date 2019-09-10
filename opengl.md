# OpenGL_Study

OpenGL website 'https://opengl.org/'


 -----------------
 
 
 ## OpenGL API 기본구조
 
 ### Open GL 함수의 기본구조
 
glVertex3f(x,y,z);
 
 1. gl (library)
 2. Vertex 점(Function Command)
 3. 3f float 값()
 4. x,y,z 축에 대한 좌표
 
 #### GL API type
 
OpenGL API | Sample Code
------------ | -------------
GL | glColor3f(1.0, 1.0, 1.0);
GLU | gluSphere(sphere, 1.0f, 50, 10);
GLAUX | auxWireSphere(0.3);
GLUT | glutWireSphere(0.8, 100, 10);

 #### Open GL Data Type
 
Suffix | Data Type | C/C++ Type | OpenGL Type
------------ | ------------- | ------------ | ------------- |
i | 32 bit integer | int or long | GLint |
f | 32 bit floating point | foat | GLfloat |
d | 64 bit floating point  | double | GLdouble |

 -----------------
 
 ### Open GL 함수의 기본구조
 
Function Name | Description
------------ | -------------
glutInitWindowSize() | Window의 크기(해상도) 설정
glutSetWindowTitle() | Window Title 설정


void glutInit (int \*argcp, char \*\*argv);
argcp
// main 함수에서 프로그램의 수정되지 않은 argc 변수에 대한 Pointer
// glutInit 함수는 GLUT Library를 위한 적절한 실행 명령어 선택옵션을 골라내기 때문에 반환값에 따라 argcp가 가르키는 값이 변경

argv
// main 함수에서 사용되는 수정할 수없는 프로그램의 argv 변수

parameter

GLUT_RGBA
//RGBA 모드 Window를 선택하기위한 Bit mask

GLUT_Double 
//Double Buffered Window를 선택하기위한 Bit mask
