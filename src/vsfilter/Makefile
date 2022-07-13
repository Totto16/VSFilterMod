


.PHONY : all

.PHONY : clean


all: Copy.cpp.o csriapi.cpp.o DirectVobSub.cpp.o DirectVobSubFilter.cpp.o DirectVobSubPropPage.cpp.o plugins.cpp.o StdAfx.cpp.o StyleEditorDialog.cpp.o systray.cpp.o TextInputPin.cpp.o vfr.cpp.o VSFilter.cpp.o 
	$(CXX) $(CXXFLAGS) -shared -o vsfiltermod.so Copy.cpp.o csriapi.cpp.o DirectVobSub.cpp.o DirectVobSubFilter.cpp.o DirectVobSubPropPage.cpp.o plugins.cpp.o StdAfx.cpp.o StyleEditorDialog.cpp.o systray.cpp.o TextInputPin.cpp.o vfr.cpp.o VSFilter.cpp.o 


%.cpp.o: %.cpp
	$(CXX) $(CXXFLAGS) -I..\..\include -I..\luajit\luajit-2.0 -I\src -I..\BaseClasses -I..\libpng -I..\zlib -I..\..\vapoursynth\sdk\include\vapoursynth -c -fPIC -o $@ $^


clean:
	$(RM) adler32.o compress.o crc32.o deflate.o gzclose.o gzlib.o gzread.o gzwrite.o infback.o inffast.o inflate.o inftrees.o trees.o uncompr.o zutil.o
	$(RM) vsfiltermod.so
