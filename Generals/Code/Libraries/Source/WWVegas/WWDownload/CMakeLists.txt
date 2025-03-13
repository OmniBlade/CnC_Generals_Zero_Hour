# Set source files
set(WWDOWNLOAD_SRC
    Download.cpp
    FTP.CPP
    registry.cpp
    urlBuilder.cpp
    Download.h
    DownloadDebug.h
    downloaddefs.h
    ftp.h
    ftpdefs.h
    Registry.h
    urlBuilder.h
)

# Targets to build.
add_library(wwdownloadg STATIC)

target_link_libraries(wwdownloadg PRIVATE
    wwcommong
)

target_sources(wwdownloadg PRIVATE ${WWDOWNLOAD_SRC})
