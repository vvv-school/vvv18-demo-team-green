# Copyright: (C) 2016 Department of Robotics Brain and Cognitive Sciences - Istituto Italiano di Tecnologia
# Authors: Vadim Tikhanoff
# CopyPolicy: Released under the terms of the GNU GPL v2.0.

file(GLOB conf    ${CMAKE_CURRENT_SOURCE_DIR}/conf/*.ini
                ${CMAKE_CURRENT_SOURCE_DIR}/conf/*.yml)

file(GLOB scripts ${CMAKE_CURRENT_SOURCE_DIR}/scripts/*.xml)

yarp_install(FILES ${conf}    DESTINATION ${ICUBCONTRIB_CONTEXTS_INSTALL_DIR}/${PROJECT_NAME})
yarp_install(FILES ${scripts} DESTINATION ${ICUBCONTRIB_APPLICATIONS_INSTALL_DIR})
