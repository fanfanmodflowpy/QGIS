IF (GRASS_NUM_VERSION6 GREATER 60300 OR GRASS_NUM_VERSION7 GREATER 60300)
FILE (GLOB MODULE_FILES *.py )
INSTALL (FILES ${MODULE_FILES}
         DESTINATION ${QGIS_DATA_DIR}/grass/scripts
	 PERMISSIONS OWNER_READ OWNER_WRITE OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE )
ENDIF (GRASS_NUM_VERSION6 GREATER 60300 OR GRASS_NUM_VERSION7 GREATER 60300)
