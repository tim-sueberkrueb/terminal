file(GLOB_RECURSE SOURCES *.cpp *.h terminal.qrc)

add_executable(liri-terminal ${SOURCES})
target_link_libraries(liri-terminal
                      Qt5::Core
                      Qt5::Qml
                      Qt5::Quick
                      Qt5::Widgets)

install(TARGETS liri-terminal
        DESTINATION ${BIN_INSTALL_DIR})
