Getting Started
===================

Getting started developing for LeagueSharp is fairly easy and best done in the IDE Visual Studio by Microsoft.
You can get the Community Edition (free) [here](https://www.visualstudio.com/en-us/products/visual-studio-community-vs.aspx)

Note: If you are completely new to programming in C# take a look at [this video tutorial](https://www.youtube.com/playlist?list=PLKFYngx4WGFeX_XxKRbC3Y3_Pxc4eIEmx) ([found by jQuery](https://www.joduska.me/forum/topic/15024-101-how-to-start-programming/))

Just follow the installer's instructions until you see this
![pic](http://gyazo.com/3d1ace1ac3741af78b40db90b52adb03)


Creating a Project
-------------

To create a new project, go to 
File -> New -> Project
and select (C#) Console Application 

Visual Studio will now automatically generate a basic program body for you

    using System;
	using System.Collections.Generic;
	using System.Linq;
	using System.Text;
	using System.Threading.Tasks;
	
	namespace ConsoleApplication1
	{
	    class Program
	    {
	        static void Main(string[] args)
	        {
	        }
	    }
	}

The method `static void Main(string[] args)` is our program's entry point.
But first, we need to include LeagueSharp as a reference in order to properly work with it.

To do this, locate the solution explorer (default on the right side).
You will see you current project "ConsoleApplication1" containing the file "Program.cs", which we just looked at, as well as an entry named "References".
Right click that and choose "Add Reference".

A new window will pop up.
Select "Browse" and locate following files on your computer:

> LeagueSharp.dll
> LeagueSharp.Common.dll
> SharpDX.dll

Tick them and click "OK",

-----------------

That's it!
You are now set up to create your first assembly with LeagueSharp.
Continue with [Creating a Hello World application](xxx)
 