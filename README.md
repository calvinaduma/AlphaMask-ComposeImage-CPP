Calvin Aduma

This program:
- reads and writes images using OIIO
- converts image 3 channels to 4 channels
- converts RGB to HSV
- green screen masks
- composites an image on top of another


alphamask:

  Uncomment these lines:
  #this will be the name of your executable
  #PROJECT = alphamask

  #list a .o file for each .cpp file that you will compile
  #this makefile will compile each cpp separately before linking
  #OBJECTS = alphamask.o

  #this does the linking step
  #alpha: ${PROJECT}
  #${PROJECT} : ${OBJECTS}
  #	${CC} ${CFLAGS} -o ${PROJECT} ${OBJECTS} ${LDFLAGS}

  and comment these lines:
  #PROJECT2 = compose
  #OBJECTS2 = compose.o
  #compose: ${PROJECT2}
  #${PROJCT2} : ${OBJECTS2}
  #	${CC} ${CFLAGS} -o ${PROJECT2} ${OBJECTS2} ${LDFLAGS}

  then run "make clean" followed by "make"

compose:
  Comment these lines:
  #this will be the name of your executable
  #PROJECT = alphamask

  #list a .o file for each .cpp file that you will compile
  #this makefile will compile each cpp separately before linking
  #OBJECTS = alphamask.o

  #this does the linking step
  #alpha: ${PROJECT}
  #${PROJECT} : ${OBJECTS}
  #	${CC} ${CFLAGS} -o ${PROJECT} ${OBJECTS} ${LDFLAGS}

  and uncomment these lines:
  #PROJECT2 = compose
  #OBJECTS2 = compose.o
  #compose: ${PROJECT2}
  #${PROJCT2} : ${OBJECTS2}
  #	${CC} ${CFLAGS} -o ${PROJECT2} ${OBJECTS2} ${LDFLAGS}

  then run "make clean" followed by "make"
  
  The program allows you to pick your hue, saturation, and value numbers to test the green screen. You may input values yourself to create your own mask.
