foreach(prog imcollapse imfit)
    add_executable (${prog}  ${prog}.cc)
    target_link_libraries (${prog} casa_imageanalysis ${CASACORE_ARCH_LIBS})
    install(TARGETS ${prog} DESTINATION bin)
endforeach(prog imcollapse imfit)
