# Target specific macros
TARGET = main
TARGET_SOURCES = $(addprefix src/, \
	main.c types.c directions.c lightsensor.c movements.c RobotHandler.c algo/Algo.c algo/AStarNode.c algo/AStarPathFinder.c algo/DeadEndHandler.c algo/MazeArray.c algo/Node.c)
TOPPERS_OSEK_OIL_SOURCE = ./main.oil

# Don't modify below part
O_PATH ?= build

UNAME := $(shell uname)
ifeq ($(UNAME), Darwin)
	INC=/Applications/robolab/nxtOSEK/toppers_osek/kernel
	include /Applications/robolab/nxtOSEK/ecrobot/ecrobot.mak
else
	INC=/cygdrive/C/cygwin/nxtOSEK/toppers_osek/kernel
	include /cygdrive/C/cygwin/nxtOSEK/ecrobot/ecrobot.mak
endif



