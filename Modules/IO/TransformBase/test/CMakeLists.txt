itk_module_test()
set(ITKIOTransformBaseTests
itkTransformFileReaderTest.cxx
itkTransformFileWriterTest.cxx
itkTransformFactoryBaseTest.cxx
)

CreateTestDriver(ITKIOTransformBase "${ITKIOTransformBase-Test_LIBRARIES}" "${ITKIOTransformBaseTests}")

itk_add_test(NAME itkTransformFileReaderTest
      COMMAND ITKIOTransformBaseTestDriver itkTransformFileReaderTest)
itk_add_test(NAME itkTransformFileWriterTest
      COMMAND ITKIOTransformBaseTestDriver itkTransformFileWriterTest)
itk_add_test(NAME itkTransformFactoryBaseTest
      COMMAND ITKIOTransformBaseTestDriver itkTransformFactoryBaseTest)
