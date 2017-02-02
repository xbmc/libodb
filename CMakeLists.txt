cmake_minimum_required(VERSION 3.2)

project(libodb VERSION 2.4.0 LANGUAGES CXX)

if(MSVC)
  set(CMAKE_DEBUG_POSTFIX d)
endif()

add_library(libodb
${CMAKE_CURRENT_SOURCE_DIR}/odb/database.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/database.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/database.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/database.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/exception.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/exceptions.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/exceptions.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/forward.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/function-table.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-pointer-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr-impl.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr-impl.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr-impl.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/lazy-ptr-impl.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc8.vcproj
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc9.vcproj
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc10.vcxproj
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc10.vcxproj.filters
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc11.vcxproj
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc11.vcxproj.filters
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc12.vcxproj
${CMAKE_CURRENT_SOURCE_DIR}/odb/libodb-vc12.vcxproj.filters
${CMAKE_CURRENT_SOURCE_DIR}/odb/no-id-object-result.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/no-id-object-result.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/no-op-cache-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/nullable.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/object-result.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/pointer-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/polymorphic-info.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/polymorphic-map.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/polymorphic-map.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/polymorphic-map.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/polymorphic-object-result.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/polymorphic-object-result.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/post.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/pre.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/prepared-query.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/prepared-query.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/query.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/query-dynamic.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/query-dynamic.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/query-dynamic.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/query-dynamic.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/result.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/result.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/result.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/schema-catalog.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/schema-catalog.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/schema-catalog-impl.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/schema-version.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/section.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/section.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/session.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/session.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/session.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/session.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/simple-object-result.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/simple-object-result.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/statement.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/statement.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/statement-processing.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/statement-processing-common.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-array-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-deque-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-forward-list-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-list-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-map-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-set-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-unordered-map-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-unordered-set-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/std-vector-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tracer.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tracer.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/transaction.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/transaction.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/transaction.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector-impl.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector-impl.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector-impl.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/vector-traits.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/version.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/view-image.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/view-result.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/view-result.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/wrapper-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/cache-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/callback.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/callback.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/connection.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/connection.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/connection.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/connection.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/container-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/core.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/compilers/vc/pre.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/compilers/vc/post.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/config-vc.h
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/c-string.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/exception.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/export.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/function-wrapper.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/function-wrapper.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/function-wrapper.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/lock.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/lock.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/mutex.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/mutex.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr-fwd.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/thread.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/tls.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/transfer-ptr.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/type-info.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/unique-ptr.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/unused.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/wrapper-p.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/buffer.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/buffer.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/condition.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/condition.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/config.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/remove-volatile.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/static-assert.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/answer.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/class-p.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/polymorphic-p.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/remove-const.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/remove-const-volatile.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/meta/remove-pointer.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr/base.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr/counter-type.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr/exception.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr/base.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr/base.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/shared-ptr/base.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/exceptions.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/exceptions.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/init.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/init.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/lock.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/mutex.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/mutex.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/once.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/once.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/once.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/once-init.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/thread.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/thread.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/tls.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/tls.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/tls.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/tls.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/tls-init.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/windows.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/condition.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/condition.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/condition.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/details/win32/dll.cxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/wrapper-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/lazy-pointer-traits.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/lazy-ptr.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/lazy-ptr.ixx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/lazy-ptr.txx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/memory.hxx
${CMAKE_CURRENT_SOURCE_DIR}/odb/tr1/pointer-traits.hxx
)

target_include_directories(libodb
  PRIVATE
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
  INTERFACE
  $<INSTALL_INTERFACE:include/odb>
  PUBLIC
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/odb>
)

target_compile_definitions(libodb
  PRIVATE
  _CRT_SECURE_NO_WARNINGS
  _CRT_STDC_NO_DEPRECATE
  _USRDLL
  LIBODB_DYNAMIC_LIB
)

include(CMakePackageConfigHelpers)
write_basic_package_version_file(
  ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}-config-version.cmake
  VERSION ${PROJECT_VERSION}
  COMPATIBILITY AnyNewerVersion
)

install(TARGETS libodb EXPORT libodb
  RUNTIME DESTINATION bin
  ARCHIVE DESTINATION lib
  LIBRARY DESTINATION lib
)

install(DIRECTORY
  ${CMAKE_CURRENT_SOURCE_DIR}/odb
  DESTINATION include
  PATTERN *.cxx EXCLUDE
)

install(EXPORT libodb
  FILE
  ${PROJECT_NAME}.cmake
  NAMESPACE
    ${PROJECT_NAME}::
  DESTINATION
    lib/cmake/${PROJECT_NAME}
)

install(FILES
  cmake/${PROJECT_NAME}-config.cmake
  ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}-config-version.cmake
  DESTINATION
    lib/cmake/${PROJECT_NAME}
)

export(TARGETS libodb
  FILE
  ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}-config.cmake
  NAMESPACE ${PROJECT_NAME}::
)