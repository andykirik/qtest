get Qt on Linux:
	wget http://download.qt.io/official_releases/online_installers/qt-unified-linux-x64-online.run
	chmod +x qt-unified-linux-x64-online.run 
	./qt-unified-linux-x64-online.run 

	sudo apt-get install libqt5-qtbase-devel

build on Linux:
	cmake .. [-DCMAKE_PREFIX_PATH=/home/jsguru/Qt/5.13.0/]
	cmake --build .
