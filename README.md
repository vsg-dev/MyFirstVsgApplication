# MyFirstVsgApplication
Very simple crossplatform CMake, C++17 project to illustrate how to build a [VulkanSceneGraph](https://github.com/vsg-dev/VulkanSceneGraph) application.

## Checkout repository:

    git clone https://github.com/vsg-dev/MyFirstVsgApplication.git

## Unix and macOS build:

    cd MyFirstVsgApplication
    cmake .
    make

## Windows build:

According to community feedback it's working fine under Windows, but we're waiting on a Windows expert to volunteer an explanation, in the meantime have a look through the [VulkanSceneGraph/INSTALL.md](https://github.com/vsg-dev/VulkanSceneGraph/blob/master/INSTALL.md#detailed-instructions-for-setting-up-your-environment-and-building-for-microsoft-windows).

## Running the MyFirstVsgApplication program:

To run, pass a 3d model to load via the command line:

    bin/myfirstvsgapplication models/lz.vsgt

This is what you should see:

![myfirstvsgapplication lz.vsgt](https://raw.githubusercontent.com/vsg-dev/MyFirstVsgApplication/master/images/myfirstvsgapplication_lz.png)


If you build just the VulkanSceneGraph then you'll only be able to load VulkanSceneGraph native .vsgt and .vsgb files, but if you've built and installed [osg2vsg](https://github.com/vsg-dev/osg2vsg) and [vsgXchange](https://github.com/vsg-dev/vsgXchange) prior to building MyFirstVsgApplication, cmake will automatically find these and add the required links and C++ to leverage all the loaders provided by the OpenSceneGraph and vsgXchange.

## Support and developer Discussion:

If you have any questions about this example program or the VulkanSceneGraph please use the VulkanSceneGraph/discussions on Github and post your questions there: https://github.com/vsg-dev/VulkanSceneGraph/discussions
