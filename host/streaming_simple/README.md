Stream Simple
======================

This is a simple Vector Add C Kernel design with 2 Stream inputs and 1 Stream output that demonstrates on how streaming kernel can be implemented and how host can directly send data to kernel without global memory.

***KEY CONCEPTS:*** Read/Write Stream, Create/Release Stream

***KEYWORDS:*** cl_stream, CL_STREAM_EOT, CL_STREAM_NONBLOCKING

## SUPPORTED PLATFORMS
Platform | Board             | Software Version
---------|-------------------|-----------------
xilinx_u200_qdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u250_qdma|Xilinx Alveo U250|VITIS 2019.2


##  DESIGN FILES
Application code is located in the src directory. Accelerator binary files will be compiled to the xclbin directory. The xclbin directory is required by the Makefile and its contents will be filled during compilation. A listing of all the files in this example is shown below

```
src/host.cpp
src/krnl_stream_vadd.cpp
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./vadd_stream <krnl_stream_vadd XCLBIN>
```

