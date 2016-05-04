cmake_minimum_required(VERSION 2.8)
 
project(HelloWorld)
 
include_directories("I:\\PhD\\software\\FANN_neural\\src\\src\\include")  
link_directories("I:\\PhD\\software\\FANN_neural\\src\\bin\\Win32")
 
add_executable(HelloTrain HelloTrain.cxx)
add_executable(HelloExec HelloExec.cxx)


target_link_libraries(HelloTrain fanndouble.lib fanndoubled.lib fannfixed.lib fannfixedd.lib fannfloat.lib fannfloatd.lib)
target_link_libraries(HelloExec fanndouble.lib fanndoubled.lib fannfixed.lib fannfixedd.lib fannfloat.lib fannfloatd.lib)