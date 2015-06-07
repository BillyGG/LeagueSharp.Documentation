Adding References to LeagueSharp
===================

What is a reference?
-------------
In order to use a component in your application, you must first add a reference to it. Visual Studio provides five options in the Add Reference dialog box:    

 - .NET lists all .NET Framework components available for referencing.

    

 - COM lists all COM components available for referencing.

    

 - Projects lists all reusable components created from local projects.

    

 - Browse enables you to browse for a component in the file system.

    

 - Recent contains a list of components recently added to projects on
   your computer.

[[More information]](https://msdn.microsoft.com/en-us/library/wkze6zky.aspx)

----------

Let's begin.
-------------
Open up your C# project file, or create a new one.

Find your 'Solution Explorer'   (View > 'Solution Explorer' / CTRL + W > S).
Once opened, it should look similar to the image below:

![Solution Explorer](http://i.gyazo.com/fe1c65b113064d8320d28d5818bd30da.png)

----------

Adding a reference.
-------------
Now that you have found the 'Solution Explorer' we can start adding our references to our project.

In the list elements, you can easily see 'References'.
Right clicking this, we are given a number of options, the one we want is 'Add Reference'.

![Add Reference](http://i.gyazo.com/506f300b0f2f82be298afba2df657467.png)

![Reference Manager](http://i.gyazo.com/6d7af19233af7ec915dc590c463330f1.png)

It is now time to add your references.

First, head to the 'Browse' section on the left, followed by the 'Browse...' button in the bottom right.

You then want to select the three main .dll files using CTRL/CMD + Click

> LeagueSharp.Common.dll
> LeagueSharp.dll
> SharpDX.dll

Then press OK to close the explorer.
Make sure the tick boxes next to the references are ticked to add them to your project, once you're done, press OK.

----------

Using references in your classes
-------------

Open up your main class file from the 'Solution Explorer'. e.g. Program.cs

You will then be met with code that is extremely similar to this:

	using System;
	using System.Collections.Generic;
	using System.Linq;
	using System.Text;
	using System.Threading.Tasks;

	namespace LeagueSharp Assembly
	{
	    class Program
	    {
	    }
	}

What we will be focusing on is the top part:


	using System;
	using System.Collections.Generic;
	using System.Linq;
	using System.Text;
	using System.Threading.Tasks;

These are references that have been automatically added by Visual Studio, you can use these as a template for adding your own.

Underneath the last one, add the word `using`followed by the name of the reference we added earlier, and ending it with a `;`

Here is what it should look like after you've added all three.

    using System;
    using System.Collections.Generic;
    using System.Linq;
    using System.Text;
    using System.Threading.Tasks;
    using LeagueSharp;
    using LeagueSharp.Common;
    using SharpDX;
    
    namespace LeagueSharp Assembly
    {
        class Program
        {
        }
    }

