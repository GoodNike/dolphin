remove_definitions(-DTRANSLATION_DOMAIN=\"dolphin\")
add_definitions(-DTRANSLATION_DOMAIN=\"dolphin_servicemenuinstaller\")

add_executable(servicemenuinstaller servicemenuinstaller.cpp)
target_link_libraries(servicemenuinstaller PRIVATE
    Qt5::Core
    KF5::I18n
)
install(TARGETS servicemenuinstaller ${KDE_INSTALL_TARGETS_DEFAULT_ARGS})
