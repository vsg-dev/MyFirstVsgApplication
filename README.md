# MyFirstVsgApplication
Very simple project to illustrate how to build a [VulkanSceneGraph](https://github.com/vsg-dev/VulkanSceneGraph) application.

This is very early days for this little example so it's only tested under Linux so far, we need others in the developer community to get things working under Windows and macOS. The repository has been setup in github to allow you to use it as template for your own applications.

## Checkout repository:

    git clone https://github.com/vsg-dev/MyFirstVsgApplication.git

## Unix build:

    cd MyFirstVsgApplication
    cmake .
    make

## Windows build:

    Please help port this application to Windows and provide text to go here :-)


## Running the MyFirstVsgApplication program:

To run pass the 3d model to load via the command line:

    bin/myfirstvsgapplication models/lz.vsgt

This is what you should see:

![myfirstvsgapplication lz.vsgt](https://raw.githubusercontent.com/vsg-dev/MyFirstVsgApplication/master/images/myfirstvsgapplication_lz.png)


If you build just the VulkanSceneGrah then you'll only be able to load VulkanSceneGraph native .vsgt and .vsgb files, but if you've built and installed [osg2vsg](https://github.com/vsg-dev/osg2vsg) and [vsgXchange](https://github.com/vsg-dev/vsgXchange) prior to build MyFirstVsgApplication cmake will automatically find these and add the required links and C++ to leverage all the loaders provided by the OpenSceneGraph and vsgXchange.

## Support and developer Discussion:

If you have any questions about this example program and the VulkanSceneGraph please subscribe to the vsg-users googlegroup and posty your questions there: https://groups.google.com/forum/#!forum/vsg-users

