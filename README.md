# Welcome to the BEST Digital SAT Prep EVER MADE!

First things first, a lot of information used for this was taken from the OFFICIAL DIGITAL SAT PREP FROM KHAN ACADEMY, with many additions and many, many changes. This is NOT a COMPLETE replacement of Khan Academy. It's more like an addition. Kinda. This covers all the text and visual part of Khan
Academy, but the practice questions are not included. I felt like they're perfect on Khan Academy as they are. So you can learn *here* and solve *there*. 

### Important note
The SAT is not hard. Whatever you've heard is false. It is, no joke, LAUGHABLY easy. I was surprised at how easy it was. Especially the Math section. 

### Back to the main point

Khan Academy is the Official Source to prepare for the Digital SAT. And that is what I used. It is GREAT, but it has its flaws and drawbacks. So, as a student who understands the SAT, (and although I bought a LOT of unofficial prep books which I never used) I felt like there was no ONE singular source where all the information about the Digital SAT was available FREELY for everyone to access. 

So I created it. This is the ultimate SAT repository.

I am a student who drastically improved his score (250 points as of August 1st) by only studying from Khan Academy for the SAT.

I got 1300 as a diagnostic.

I got 1440 on my December attempt, and I  I honestly expected to get a 1570, but then realized that I needed to work a bit harder for that.

I got a 1490 in March.

I got a 1550 in June, with a breakdown of 800 for Math and 750 for English.

And I am going to be giving the August SAT, with a goal of 1600. We'll see what the outcome is soon!

Back to the part where this is to help YOU. Since I'm a student, I really do not want this to be closed behind a paywall to other students. Rather, it should be spread far and wide so that as many people can benefit from it as possible. So share it with your friends! Let them know! 

Now, Khan Academy "will walk you through the digital SAT assessment, providing articles, video lessons, and exercises covering every type of question you might see on the test.... practising on Khan Academy can sharpen your skills, boost your confidence, and ensure that you’re prepared for anything the test might throw at you."

But, what they assume is prior knowledge of certain concepts and skills, among other small details I've noticed while I learnt for the SAT from Khan Academy myself.

I won't be doing that. I'll provide as much background information as possible, and I am making this on Jupyter Notebook so that I can create and add whatever diagrams I want on the go without any effort.

# According to Khan Academy, the best way to prepare for the SAT is:
*Taken from Khan Academy btw*


Khan Academy’s Official Digital SAT Prep includes thousands of SAT Math questions and hundreds of SAT Reading and Writing questions developed by the test-maker, College Board, and loaded with insightful lessons and explanations written by Khan Academy’s test prep experts. Before jumping into practice, though, we recommend getting familiar with the format of the test, the content of the test, and the digital platform on which the test is administered by taking a full-length practice test. *Note: (The platform is Bluebook, which you can download for free by going to the Official College Board Site)*



That is completely accurate and I could not agree more. I literally told everyone who asked me from where I studied for the SAT never to use any external sources but to rather only use Khan Academy (And the official book). BUT, this is for practicing questions, not learning concepts. That's where I come in with this. I repeat, learn here, solve there.


There are two main components to getting that sweet, sweet perfect score: Full-length practice tests and Skill Practice

### Full-length practice tests

Full-length practice tests give you the best idea of what test day will be like, offering the ideal opportunity to both test your skills and become familiar with the testing platform. You can take full-length practice tests using College Board’s Bluebook app. After taking each practice test, you can review your performance and read answer explanations for the questions you missed. *(You will get in-depth answer explanations on Khan Academy, and that is one of the reasons this is not a replacement of Khan Academy. It is still an indispensable resource.)*

It is highly recommended to take full-length practice tests at set intervals throughout your test prep journey. Starting with a practice test will allow you to diagnose the areas where you need the most practice. Future practice tests will allow you to gauge your progress, refine the focus of your skill practice, and build endurance and experience for test day.

### Skill practice

Skill practice is basically the solving part. You have to try all the different types of SAT questions, use the multiple different strategies I will provide for answering those questions, and practice the skills that those questions test. The best way to practice individual skills is to explore both the digital SAT Math course and the digital SAT Reading and Writing course on Khan Academy. You can read articles and watch videos covering each skill, and then you can practice those skills and test yourself in the related exercises. As you become proficient in more skills, you’ll become more prepared for test day.

So let's begin your SAT journey with a BANG! *Or for some of you, hopefully, almost the end of it!*

And as Sal always says...
# Good luck! You’ve got this.






import matplotlib.pyplot as plt
    from mpl_toolkits.mplot3d import Axes3D
    
    # Data
    verbs = ['be', 'have', 'do', 'say']
    tenses = ['1st Pres', '3rd Pres Sg', 'Plural Pres', '1st Past', 'Plural Past']
    conjugations = [
        ['I am', 'she is', 'we are', 'I was', 'we were'],
        ['I have', 'she has', 'we have', 'I had', 'we had'],
        ['I do', 'she does', 'we do', 'I did', 'we did'],
        ['I say', 'she says', 'we say', 'I said', 'we said']
    ]
    
    # Create figure
    fig = plt.figure()
    ax = fig.add_subplot(111, projection='3d')
    
    # Plot data
    for i, verb in enumerate(verbs):
        for j, tense in enumerate(tenses):
            ax.text(i, j, 0, conjugations[i][j], color='magenta', ha='center')
    
    # Set labels
    ax.set_xticks(range(len(verbs)))
    ax.set_xticklabels(verbs)
    ax.set_yticks(range(len(tenses)))
    ax.set_yticklabels(tenses)
    ax.set_zticks([0])
    ax.set_zticklabels(['Conjugation'])
    
    # Set axis labels
    ax.set_xlabel('Verb')
    ax.set_ylabel('Tense')
    ax.set_zlabel('')
    
    plt.show()
