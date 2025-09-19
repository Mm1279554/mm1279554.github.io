# My Codeing Notebook

## Table of Contents
- [Flutter Notes ](#day-1)
  - [what-is-flutter](#what-is-flutter)
  - [Key terms and Definitions ](#key-terms-and-definitions)
- [Code Definitions](#code-definitions)
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

## Flutter Notes

### What is Flutter?
- Definition: A framework made by Google for building apps that work on web, Android, and IOS -with one codebase.
- Why is it useful? Used the Dart programing language.

---

### Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | Basic building block of a FLutter app. Everything is a widget                                                  | Text, Image,Container, Column                                           |
| MaterialApp      | The root of the app. Sets up routes and themes.                                                  | Found in main . dart                                           |
| Scaffold         | Provides basic visual layout - like a header, body, floating button                                                 | Each screen uses it                                           |
| StatelessWidget  | A widget that dosent change                                                  | Most of the screen files                                           |
| StatefulWidget   | A widget that can chnage over time                                                  | Used in MyHomePage( )                                           |
| Navigator        | Manages screen transitions                                                   | Navigator .pushNamed( context, '/page2');                                           |
| AppBar           | Top navigation bar                                                 | Title of each page appears here                                           |
| Column           | Vertical layout                                                  |                                           |
| Row              | Horizontal layout                                                 |                                           |
| Container        | Wraps content with padding, margin, or color                                                 |                                           |
| Text             | Displays text                                                 |                                           |
| Image.network    | Displays images from a URL                                                 |                                           |

| Padding    | Adds space around a widget                    |                     |

| Center | Centers its child                        |                     |

---

### Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?







## Flutter Definitions with structures

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|Main      | A function that runs when your app starts. It tells Flutter what app to show. | |A car starts up  |in main.dart, void main() => runApp(MyPortfolioApp());  |
|      | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |  |main.dart,return MaterialApp( debugShowCheckedModeBanner: false,title: 'TSA Portfolio',theme: ThemeData(  |
|      | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |  | in showcase. dart, return Scaffold(body: Column(mainAxisAlignment: MainAxisAlignment.start,children: [  |
|      | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |  |in showcase.dart, body: Column( mainAxisAlignment: MainAxisAlignment.start, children: [   |
|      | A widget that shows things side-by-side. | `Row(...)` |  |in InfoCard.dart, child: Row(children: [ClipRRect(borderRadius: BorderRadius.circular(8),child: Image.network(imageUrl, width: 100, height: 100,fit:BoxFit.cover),   |
|Container      | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |On canva you open a new project have a container to add new designs  |In infoCard.dart, return Container(margin: const EdgeInsets.symmetric(vertical: 8, horizontal: 16),padding: const EdgeInsets.all(12),decoration: BoxDecoration(  |
|Text      | A widget to display text on the screen. | `Text('Hello')` |When you text your mom  |In InfoCard.dart, child: Text(description,style: const TextStyle(color: Colors.white),  |
|Image.network      | A widget to show an image using a link from the internet. | `Image.network('https://...')` |It takes up less space  |In Infocard.dart, child: Image.network(imageUrl, width: 100, height: 100, fit: BoxFit.cover),  |
|ElevatedButton      | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |Press the button the video starts playing  |In home.dart, ElevatedButton(onPressed: () => Navigator.pushNamed(context, '/background'),  |
|onPressed      | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |onpressed take me to the next slide  |In home.dart, onPressed: () => Navigator.pushNamed(context, '/background'),child: const Text('Next'),  |
|StatelessWidget      | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |Welcome page and about me page dosent have to be changed  |In home.dart, class HomeScreen extends StatelessWidget {const HomeScreen({super.key});  |
|Navigator      | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |Takes me to next slide or next youtube video  |In   |
|@override      | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |When we want to customize override build method so how we want it to be but not chnage behavior  |  |
|Paddding      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |Padding to push off center and makes space   |  |
|Center      | Aligns content in the center of the screen or container. | `Center(child: ...)` |Welcome to this app to be in the center  |  |
|Wrap     | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |Wrtiting text going to wrap it to the next line  |  |
|override      | This marks a method as one that’s replacing a method in a parent class. | `@override` |  |  |
|Build      | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |Define that screen and build it shows up  |  |
|BuildContext      | Required in every widget class to describe what to show. | `build` |Move between tabs and the build context tracks where your at  |  |
|    | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |  |
|Super.key      | A keyword used to pass a value to the parent widget. | `super.key` |email your teacher you are sending information and they are above  |  |
|const      | A keyword that means the value won't change and is set once. | `const` |Cant change the code while its running  |  |







## Code Definitions

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
|Variable      | A named container used to store a value that may change. | `var x = 5;` |  |  |
|Constant      | A fixed value that cannot change once set. | `const PI = 3.14;` |  |  |
|Data Type      | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` |  |  |
|String      | A sequence of characters used to represent words or text. | `"Hello World"` |  |  |
|Integer      | Whole number values. | `int age = 16;` |  |  |
|Double      | Number values with decimals. | `double age = 16.2;` |  |  |
|Boolean      | A value that can be true or false. | `bool isLoggedIn = false;` |  |  |
|List      | A collection of values in a specific order. | `List<String> names = [];` |Calendar  |  |
|Null      | A special value that means “nothing.” | `String? name = null;` |When you register for school your classes are null but they have the placeholders  |  |
|Function      | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |Have a light switch the turn on all the lights or on wthat only turn on one light  | |
|Parameter      | The information passed into a function to change how it works. | `greet(String name)` |If I log in to tiktok or instagram I am the parameter  ||
|Return      | The result a function gives back. | `return total;` |If you go to the bank and you finished you get a recipt  |  |
|Scope      | Where a variable or function can be used. | (No set syntax — concept-based) |If you have a starbucks gift card you can only use at starbucks that is the scope  |  |
|Class      | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |Take notes complete work  |  |
|Object      | A specific version of a class. | `Dog myDog = Dog();` |20 students they are all objects  |  |
|Property      | A variable that belongs to a class/object. | `String name;` |Water bottle has a capacity and name age belongs to a person  |  |
|Method      | A function that belongs to a class. | `void bark() {}` |Complete homework writing notes  |Jump method belongs to people not table and chair |
|Constructor | A special function used to set up a class when it’s created. | `Dog(this.name);` |Name of baby on a birht certificate  |Makeing a project and nameing your project  |
|Abstraction      | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |Like driving a car just press the gas  |  |
|Override      | Changing how a built-in or inherited function behaves. | `@override` |Waterbottle blue and 40 oz capacity |Shaq dunking then mr davidson dunking  |
|Void      | A function that does not return a value. | `void printMessage() {}` |Turn lights on   | |













## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
