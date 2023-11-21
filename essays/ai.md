---
layout: essay
type: essay
title: "Eyes on Artificial Intelligence"
# All dates must be YYYY-MM-DD format!
date: 2023-11-21
published: true
labels:
  - Software Engineering
  - Artificial Intelligence
  - Education
---

<img width="300px" class="rounded float-start pe-4" src="../img/ai/grid-AI.jpg">

After the popularization of Chat-GPT in the Fall of 2022, there was a swift and largely negative reaction to the arrival of AI in the classroom. All of a sudden, students had a new tool that could transform the way they learned in class; for better or for worse. Many people were quick to express their distaste with the ability for students to write an entire essay with a single prompt or answer, leading them to completely write off AI as a productive learning tool. In many of my Computer Science classes, AI was included in the syllabus under the section of  “Academic Dishonesty” as students had started using it to complete entire coding assignments. That is why, on the first day of Software Engineering class, I was surprised when my professor stated that we were allowed and even encouraged to use AI throughout the semester. As a result, I have experimented with different ways to use AI, some of which I found to be productive, while others had a negative impact on my learning experience. In essence, I started out using AI for quick and easy answers and transitioned to a more understanding and reminder based approach with Chat GPT.


<br/>

## Personal Experience with AI:
<hr >

### Experience WODs

During experience WODs, I felt like I had my most unproductive uses of AI. Since I was still in the process of learning new coding concepts while doing these WODs, there were some in which I had a lot of trouble on the first attempt. Within the last couple of minutes, I would try a last ditch effort to complete it.

In particular, during E18: Experience Functional Programming (Part 1), I asked the following question with about two minutes left of time:

In javascript: Create a variable called testData and set it equal to the first few elements of the uhdata array. Use this variable to check that your functions work correctly before running them on the full data set.

Use the functions provided by the underscore package to implement the following two functions. Note that your solutions cannot include a for loop or an if statement!

totalDegrees(data). This function is passed a data structure like uhdata and returns the total number of degrees awarded in the data set. For the uhdata set, the correct answer is 48,186.

I actually got a working solution out of this prompt. However, by the time I fixed what little problems there were, the time was already up. Using AI in this way was overall unproductive.

### In-class Practice WODs

For the in class practice WODs, I used chat gpt in the same way as I used it in the Experience WODs. In the last five or so minutes of the WOD, my function was not working so I put ChatGPT to the task of figuring out what was wrong:

Fix this javascript code to give me the first 50 fib numbers:

```javascript
function fib(n, arr) {
  // eslint-disable-next-line no-prototype-builtins
  if (arr.hasOwnProperty(n)) {
    return arr[n];
  }
  if (n === 0) {
    return arr.push(0);
  }
  if (n === 1) {
    return arr.push(1);
  }
  return arr.push(fib(n - 1, arr) + fib(n - 2, arr));
}

function memoize() {
  const arr = [];
  fib(50, arr);
  return arr;
}
console.log(memoize());

```
After inputting this prompt, ChatGPT provided a correct solution and broke down each of the changes made:

We changed arr.hasOwnProperty(n) to arr[n] !== undefined to check if the value at index n is already calculated in the array.
We removed the return statements after arr.push() as arr.push() returns the new length of the array, not the value that was pushed.
In the memoize function:

We changed the loop to start from 2 (since we've already handled 0 and 1) and calculate the Fibonacci numbers up to the 50th number.
Now, when you call memoize(), it will generate the first 50 Fibonacci numbers and return an array containing those numbers.

I was a lot more successful with this last minute use of ChatGPT. I especially like how it broke down every change and explained why each was made. Even so, I still feel like if you are to use ChatGPT for the WODs, you should not keep it as a last resort and instead, commit to using it from the beginning so that you use it to efficiently build a successful solution instead of rushing to fix a broken one.

### In-class WODs

For all of the In-class WODs, I never ended up using Chat GPT. I think with all the practice WODs and Experience WODs, I always felt confident enough to do the actual WOD without the help of AI. Furthermore, I felt like these WODs were the place to really test your knowledge and so I only wanted to save AI as a last resort.

### Essays

For the essays in this class, Chat GPT has been a wonderful tool for making sure my punctuation is used correctly and reaffirming the quality of various essay components.
For the essay on Javascript, I asked:

Does this sentence use a semicolon correctly: Just like Python, JS is a dynamically typed language; meaning that you do not need to declare the data type of a variable explicitly and the type of the variable can change at runtime.”

Chat GPT Responded:

Yes, the semicolon in the sentence is used correctly. It's used to separate two related independent clauses. Independent clauses are complete thoughts that can stand alone as sentences, but they are often connected using punctuation to show their relationship. In your sentence, the semicolon appropriately connects the two clauses about JavaScript being a dynamically typed language and its characteristics.

With this response, not only did I get confirmation that my sentence used a semicolon correctly, but I was also reminded of when exactly to use this form of punctuation.

### Final Project
So far, I have not used any forms of AI for the Final Project. However, that may change as the project progresses and I need to refresh my memory of some of the concepts I learned in Software Engineering.

### Learning a Concept / Tutorial

There was one instance where I used AI for this case. When writing my JavaScript essay, I had forgotten what exactly a dynamically typed language refers to.
I asked Chat GPT:

Does dynamically typed refer to syntax or an underlying rule.

Chat GPT responded:

"Dynamically typed" refers to an underlying rule or characteristic of a programming language, not to syntax. It describes how the language handles data types for variables during program execution.

In a dynamically typed language, the type of a variable is determined and can change at runtime based on the value it currently holds. This behavior is enforced by the language's runtime environment and is not tied to specific syntax.

It then gave me an example and provided further clarification.

I found that using AI in this way was an efficient way to refresh my memory on coding concepts that I had learned in the past. The clarification provided was easily digestible and the example provided further enhanced my understanding. Although I did not use AI for learning any new concepts, I have in other classes by asking ChatGPT to explain things that are not quite clear in different words.

### Answering a question in class or in Discord

I did not use AI for this because I felt like if the question was easily answerable by AI, the person that asked the question would not resort to asking the question in discord.


### Coding Example

I never explicitly asked ChatGPT to give me an example. Often, when I need help understanding a specific code component, I would automatically receive examples from the chat bot. When I was first learning html and css, I needed a lot of help understanding various css styles and html components. One things that I asked was:

How does auto work?

In which it responded with explanations and examples for each use of “auto”:

1. Margin and Padding:

When 'auto' is applied to 'margin' or 'padding' property (for left and right margins), it automatically calculates the margin or padding space to distribute equally on both sides of an element, thus centering it horizontally within its parent container.

```css
.example {
  margin: 0 auto; /* Centers horizontally */
}
```
Using AI in this way was a very effective method for efficiently parsing through all of the different styles and html elements. Although documentation of CSS exists, I felt as though ChatGPT communicated the use of the this style more effectively than some of the documentation I found online:

auto: The browser will calculate and select a width for the specified element.

### Explaining Code

I definitely found it helpful for ChatGPT to explain code to me. For example, I asked:

What do these lines do:

```javascript
const [hideCompleted, setHideCompleted] = useState(false);

  const hideCompletedFilter = { isChecked: { $ne: true } };

  const tasks = useTracker(() =>
    TasksCollection.find(hideCompleted ? hideCompletedFilter : {}, {
      sort: { createdAt: -1 },
    }).fetch()
  );

  const pendingTasksCount = useTracker(() =>
    TasksCollection.find(hideCompletedFilter).count()
  );

  const pendingTasksTitle = `${
    pendingTasksCount ? ` (${pendingTasksCount})` : ''
  }`;
```
It responded:

The provided code appears to be part of a React component or hook that manages a to-do list. It uses React hooks like useState and useTracker and interacts with a collection named TasksCollection. Let's break down each of these lines:

const [hideCompleted, setHideCompleted] = useState(false);

1. This line uses the useState hook to create a state variable called hideCompleted and a corresponding function setHideCompleted to update its value.
2. Initially, hideCompleted is set to false, which implies that completed tasks are not hidden...

In my opinion, this was one of the best uses I found for AI since it is easy to get lost in between the lines of code, especially when you are following a tutorial and you are not quite understanding what you are writing down. It provides both a breakdown of each individual line and also wraps it up nicely with a summary at the bottom. I think more students should definitely make use of AI in this capacity since it really expedited the process of learning through code-along.

### Writing Code

This is a use that I wish I had experimented with more. I had only used AI to remember how to do small tasks such as the following:

How to use a Bootstrap icon in a Bootstrap button?

In which I got the response:

To use the Bootstrap icon bi-car-front-fill within a Bootstrap button, you can follow these steps...

In essence, I found a lot of value using ChatGPT for minor tasks like this which saved me a little bit of time searching on the web for a simple answer. I think in the future I would like to experiment more with creating coding outlines for a more complicated task. Basically, just using AI to stay organized and have a clear path to completing a big issue.

### Documenting Code

I did not really use AI to explicitly help me with documenting code. I think it just never crossed my mind to use it for documentation because that was usually something I did at the end of completing a task and by then I was comfortable enough in my understanding where I did not feel as if I had to use AI for help. However, I can definitely see AI being useful in this capacity as just like how I used it to help explain code, I could turn those explanations into documentation easily.

### Quality Assurance

For quality assurance, I have gotten mixed results. I tried using ChatGPT to help me figure out why an image was not centering correctly after I failed the Buzz’s react WOD:

In this react component, why is my image not in the center of the screen:

```jsx
const CenterImage = () => (
  <bs.Container className="justify-content-center m-5 align-items-center">
    <bs.Row>
      <bs.Col className="text-center">
        <bs.Image src="images/wod-buzzs-on+thebeach.png" width="1200px" />
      </bs.Col>
    </bs.Row>
  </bs.Container>
);
```

In which it responded:

In your code, you're using Bootstrap classes for layout, and it seems like you want to center an image within a container. Your code appears to have some issues with the Bootstrap classes.

Here's a modified version of your component to center the image:

```jsx
const CenterImage = () => (
    <bs.Container className="d-flex justify-content-center align-items-center">
      <bs.Row>
        <bs.Col className="text-center">
          <bs.Image src="images/wod-buzzs-on+thebeach.png" width="1200px" />
        </bs.Col>
    </bs.Row>
  </bs.Container>
);
```

This answer did not help me that much since the “height: 100vh” was not necessary and the image was still not centered afterwards. I found that for front end quality assurance, ChatGPT was not the most helpful. This makes sense because the chat bot cannot see what I am seeing and so it will try to solve the problem in a way that is not helpful. I found it a lot more useful to ask the professor or a peer for these types of issues.


### Other uses in ICS 314 not listed

All of the uses above encompass how I used AI in this class. Other than these uses, I can think of a few more that may have been useful such as help with writing a formal email to the professor or help with creating a resume for my professional portfolio.

## Impact on Learning and Understanding

---

Overall, I feel as if AI has had a positive impact on my learning experience in software engineering. I tried very hard not to use AI in a non-productive way, such as completing an entire assignment for me after seeing how unhelpful that was in the first set of  homework WODs. I think the biggest impact it has had was with my comprehension skills of code. Once I started learning Meteor and React, I frequently used ChatGPT to explain certain chunks of code which immensely improved my understanding of how to use these two frameworks. Although, I do not think it helped that much with skill development or problem-solving skills. For skill development, I think my retention of said skills is lacking because I could always search up how to use a certain html element or style instead of having to remember how to do certain things. As for problem solving abilities, I do not think AI helped me in this regard because it has not really taught me how to solve problems on my own. It may have even hindered this skill because AI expedites the problems solving process by immediately determining the cause of problems so that you never gain the skill necessary to look for the broken parts of your code.

## Practical Applications

---

So far, I have not personally applied AI to any outside projects in the realm of software engineering. However, I can still think of some practical applications that I may want to make use of in the future. For example, a big challenge in the software development industry is time constraints. Meeting the demands of their projects within the constraints of a deadline can lead to a lot of pressure which can tank the quality of the final product. Using AI to analyze project requirements and deadlines, potential bottlenecks can be identified and determining the priority of certain tasks can be streamlined. It can also provide insight on which tasks will require more resources or what kind of expertise is needed so that a team can effectively divide up the work to suit the strengths of each respective member. Finally, within a team environment, AI can be used to summarize group discussions  and highlight the crucial points that require the most focus.

## Challenges and Opportunities

---

The main challenge that I have encountered with the use of AI within the course is trying to separate the productive uses of AI from the unproductive uses. Each time I ask ChatGPT for help, I need to reflect on whether or not I am improving my learning experience. After completing an assignment with the help of AI, I take into consideration whether or not I fully comprehend the concepts that this assignment was trying to teach me. If not, I further reflect on whether or not the use of AI is what hindered my understanding of the concept at hand. Another challenge that I have experienced is that I don't really know if the answers that I am getting are the best they could be. Prompt engineering is a big component of utilizing AI to the best of its ability and I have never really learned the correct structure of questions to fully realize generative AI. I think it would be beneficial to try and fit in a section on prompt engineering into the Software Engineering curriculum.

## Comparative Analysis

---

Traditional teaching methods and AI enhanced approaches both have their upsides and downsides. For one, a traditional lecture based approach will not cater to every student in class. Each professor has their own teaching style which does not always align with each individual student. On the other hand, AI can provide a personalized experience to each student as long as the student is knowledgeable on how to best create a prompt to suit their specific needs. Furthermore, a lecture based class can reach upwards of 200 to 300 students. In this environment, it is impossible to give each student the required attention needed to succeed. AI can provide help and feedback to each student individually which is an educational component sorely missed in big lecture classes. However, I do not think generative AI will ever replace the effectiveness of a one-on-one exchange between a professor and a student. Although lecture styles cannot be applied to everyone, good Professors can still identify the weaknesses in each individual student and provide personalized help. I feel that this human component will always be more productive than receiving help from AI.


## Future Considerations

---

With the continued rise of AI in software engineering and education in general, I am fearful of the possibility of a future in which classes are completely taught with AI. As I said above, there will always be a need for professors that can provide human feedback and encouragement; something that AI just cannot replace. I also feel like there needs to be more education on the setbacks that may occur to one’s learning experience if they use AI in the wrong way. Many students do not know the impact that a heavy reliance on AI can have to their overall education. However, I still think that students should be encouraged to make use of AI just as they should make use of their Professors and teaching assistants. Schools should just be sure to draw a line between what is an acceptable use and what will damage one’s education.


## Conclusion

---

After experiencing an AI-integrated course for the first time, I can definitely say that AI offers transformative benefits to teaching and can revolutionize learning methods. I found that I really needed to reflect each time I used AI in class to make sure I was not ruining my learning experience and was still comprehending each concept we were taught. Classes that utilize AI need to provide ample resources to students in order to make sure they know how to use it responsibly and to the best of its ability. I think investing in more interactive AI tools could also be beneficial so that a student’s learning experience does not just become reading text off the screen. Both traditional teaching methods and an AI-integrated approach both have their strengths and weaknesses. Nevertheless, I do not see why integration cannot be made more seamless as to enhance each method together and take care of their respective weaknesses. 	
