set(LLVM_LINK_COMPONENTS
  ${LLVM_TARGETS_TO_BUILD}
  Analysis
  BitWriter
  CodeGen
  Core
  IPA
  IPO
  IRReader
  InstCombine
  Instrumentation
  MC
  ObjCARCOpts
  ScalarOpts
  Support
  Target
  TransformUtils
  Vectorize
  Passes
  TaskDebug
  )

add_llvm_tool(taskdebug
  main.cpp
  )

export_executable_symbols(taskdebug)