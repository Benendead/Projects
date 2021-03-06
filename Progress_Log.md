# Current Projects Journal
1. LSTMjazz - Working to generate jazz improv based on given chords using LSTM networks.  
Last worked on: 04/12/2019. Total time: 54h15m

11/3/2018: 1h - Spent time polishing up the very beginning of the legacy file, learning Github basics, and beginning to look into alternative/additional datasets. Today was really just to begin the cleanup needed to transition a hackathon project into an independent goal-oriented project.

11/10/2018: 1.5h - Spent this time working on installing MuseScore and Lilypond into the environment of a Colab notebook. It's quite a hassle, clearly, but my goal here is to give the notebook the ability to display PNGs of the music that's going on. I feel like this is an important piece to make the data accessible, so I'll keep working on this. I just got to the point where the two applications/packages are installed and referenced properly for music21; up next is accessing and displaying the PNG files that we're currently getting as a PosixPaths. Feels pretty close to done.

11/17/2018: 1h - Wasted the hour continuing to try to get Music21 working. At almost every turn, the documentation gives no advice for resolving errors and there's zero support in every thread I read on the library. I'll definitely plan to abandon Music21 if I can't find a way to easily parse through what are now flattened chord/note streams. It's a whole thing.

12/19/2018: 1.5h - A little over a month later, I finally got back to this project. Today I managed to parse out both chords and their durations from the .xml files. My plan moving forward is to process the .xml files through Music21 and perhaps encode the melodies using a different library. I'll look into other works more substantially before booting up Keras this time. At least today saw a bunch of progress.

12/25/2018: 2h - From yesterday into today, I've completed the chord processing method and I think the melody processing can likely take a similar approach. This is a ton of progress and hopefully I can look into the LSTM side quite soon.

12/27/2018: 1h - Reading articles on LSTMs to make sure I understand the math/theory of what I'm getting into. They seem pretty complicated, but that's not to say difficult to understand. Just a bunch of steps.

12/28/2018: 2h - Worked on formatting songs for their notes. First found ranges of songs, then adjusted those that were too low up so that they're all playable on alto sax, hypothetically. Used Matplotlib for some visuals on the ranges.  
*-10h mark-*  
12/31/2018: 1h - Revised a new version of the chord processing method as to process the notes as well. Also added labels to the notebook's graphs. All that's left is to export the arrays to .csv files and that should be data preprocessing done.

01/01/2019: 1h - Finished the first article on LSTMs, looked into a few variants of the model, and found multiple research papers I'd like to read this year. Pretty cool stuff and I'm excited to make this year my best yet for ML learning.

01/03/2019: 1h - Continued into a second article going more in-depth into backprop of RNNs and RNNs themselves. So far it's been useful yet not entirely difficult, as it's formalizing things the last article glossed over. Quite interesting so far.

01/04/2019: 1h - Still reading this second article, which is giving more insight while missing a few points in a few places. I can finish this one tomorrow and hopefully start coding within the next few days.

01/05/2019: 1h - Began reading a research paper on using char- and word-RNNs to generate jazz chord progressions. Giving me a lot of insight into using Keras for this, I'll definitely consider generating chords in my version as well.

01/06/2019: 1h - Again finished the first research paper and am into the second. These both make sense so far and continue to expand my expectations of what I'll be able to do in this project. Hyped.

01/08/2019: 2h - Spent the first hour reading the second research paper, which used LSTM to recreate a chord progression and also generate new melodies. They encoded their chords/melodies really similar to how I planned to, which is promising. In the second hour, I finished another resource explaining LSTMs and moved into another to cover my fundamentals. I also have a bunch of resources lined up to fill me in on various technical sides to LSTMs should I research into this further later.

01/09/2019: 1h - Finished the third full resource explaining LSTMs. I think my intuitions are covered and I plan to exclusively concentrate on code and applications until the project is complete. Cut out a few weak sources during the hour and also continued a marginal amount into the melody/chords LSTM application paper. I'm now somewhat close to coding, I think.

01/10/2019: 1h - I completed the first paper to use LSTMs to compose new music and am now reading something from 2010 about the use of deep belief networks (DBNs) to improvise over chords. It's a different approach but their problem is much more fundamentally mine and I should consider all possible paths forward. It's interesting to learn about another ML algorithm too. 
*-20h mark-*  
01/11/2019: 1h - Continuing the article on DBNs. Their music encoding method might be worth trying out myself.

01/12/2019: 1h - Finished the paper on DBNs and I've now continued into a massive 56-page thesis on using LSTMs to generate melodies given certain chord progressions. This is by far the most promising and relevant work I've yet seen. Exciting stuff.

01/13/2019: 2h - I spent two hours reading the thesis, working through a lot of the backprop and then explanations of RNNs and LSTMs as well as why MIDI is the better data source to use. The backprop math needed a lot of LaTeX, which took a bunch of time. I skipped the end of that section, knowing full well that it deserves more dedicated time in a later project. For now I'm into the data representation of this thesis, which is great.

01/14/2019: 1h - Continuing through the thesis; today I covered his encoding methods and data preprocessing steps. The next section regards the experiments on network topologies, which should be fascinating. This is definitely a great resource.

01/15/2019: 1h - I've finished the 56-page thesis, pretty great stuff. His approach has a few things worth looking into improving, but I'm otherwise impressed and excited to start coding my own model to attempt this problem.

01/16/2019: 2h - Over my plane flights today, I read two research papers on using LSTMs or seq-to-seq models to generate music. The first paper heavily cited the second, so upon finishing the first I read the other too. I'll need to look into the ABC data format as well as sequence-to-sequence models should I want to utilize the latter paper's (quite successful) methods. As of now, the papers are highlighted PDFs on my iPad and I'll work on typing out my notes in the next days.

01/17/2019: 1h - Continued to type up notes on the first of the papers I highlighted yesterday. I spent part of this time searching for the main author of the paper to email him a question about the methods described, and then sent the email to the student email left in the paper. Hopefully he still checks it. Regardless, I get char-RNNs now and the annealing mostly too.

01/18/2019: 2h - I've written out almost all the notes on the second paper I highlighted. It's pretty complex and I'd need to learn about Seq2Seq to improve on its full results, but the LSTM usage is still useful. I'd like to read one more additional paper with new content before combing through what I've read and beginning to write up my own plans for where to start.  
*-31h mark-*  
01/20/2019: 1h - Continuing into the last two papers (I found one with chord-based generation), I'm still looking forward to generating my own solutions. There's a necessary cutoff in researching where my own contribution is required; that point feels quite close. That's also where the real challenge begins.

01/21/2019: 1h - This paper includes some major references to music theory and I'm inclined towards thinking that such considerations should be made more often in this kind of work. Also, embedding layers have come up again which is great.

01/22/2019: 1h - Finished reading the second-to-last paper for this segment of this project. Definitely excited to do some new work of my own. I'm going to consider between a few options to make sure the last paper's useful.

01/24/2019: 1h - I've begun the summary section of my notes. My goal with this section is to identify the successes of the prior approaches I've studied while noting where they could be improved. It's the most enjoyable part in a while because I'm reading my own explanations, which is a much more easy process.

01/25/2019: 1.5h - Two more summaries done. I'll hopefully finish these this weekend, synthesize my goals as well, and then it's time to get coding. Writing the summaries continues to clarify a few of my misunderstandings from the first read-through.

01/26/2019: 1h - I finished the summary of the polyphonic succes story with Mozart and am now on the Stanford Seq2Seq paper's summary. This is the second-to-last one, will probably take a bit longer than most summaries, but the end is quite near.

01/27/2019: 1h - The summaries are complete. Compare what they've done, make my own plan, get coding. It's time.

01/29/2019: 1h - Editing my code to tranpose songs as multiple papers suggest. Once this is formatted, will export to something Keras can read in and then use. Great to be back to coding.

01/30/2019: 1h - Implemented methods to transpose everything to all 12 keys plus find the unique chords. Embedding will be ready soon, probably. Cool beans.  
*-40.5h mark-*  
01/31/2019: 1h - Continued to format chords, considering the data format constantly as to enable both bit vector and string chord representations later on in preprocessing.

02/02/2019: 1h - Token chord representations give a different number of unique chords than the bit vectors and thus I'll use the former for any kind of tonenization/embedding encoding. I'm now into writing methods to count up the number of beats each unique chord is used for across the expanded dataset.

02/03/2019: 1h - Optimization tweaks to speed up my implementations, added timers to all long processes, and created a better graph of the chord durations across all songs. Next steps should focus on the possible melody representations.

02/05/2019: 1h - Reformatting old code to transpose octaves up/down, shifting the dataset to fit within the fewest possible notes, and I wrote an overview of the varied melody encodings previous works have used.

02/06/2019: 1h - Formatting code for melodies with both piano roll and 18-bit encodings. Also developed a few preliminary methods to ensure that my encodings are robust/correct. Maybe time to put these in .csv and then Keras soon?

02/07/2019: 1h - Added code to export to .csv for everything except the dataframe-organized data. May want to consider revamping all code to directly export to dataframes, but for now adding the names lists is progress enough. Exporting soon!

02/09/2019: 1h - Revamping into dataframes, a few optimizations, and improving the graphs a bit as well. Exporting is still close, yes, but fixing everything up into a clean state is worth doing first.

02/15/2019: 1h - Adding in Seaborn, finished DataFrame revamp, and formatting the last few print statements for user clarity. Exporting next time is both a must and an easy task. Keras time...

02/19/2019: 1h - Continued attempts to get the data out of the notebook onto Github or even my own machine have still failed. The .csv are exporting into the local Colab folders fine, and I found methods to get those folders working on their own, but both pushing to Github (authentification failing) or downloading to my laptop (string formatting) have not yet worked. I'll try formatting the filenames better, maybe linking Drive, but after that I'm not sure what else to try.

02/25/2019: 1h - Uploaded datasets to Github, considering additional bit information encodings to give the LSTM an idea of where it is in each measure. This might help alleviate the issues our long-term dependencies otherwise create.
*-50.5h mark-*  
03/10/2019: 2h - Finally got back to work by studying how to sample the data for Keras and renaming the files for future convenience. Next, I'll be able to test the sampling code I wrote today.

04/12/2019: 1h45m - Coded sample method done, infrastructure to import data, and the Keras model has been started. Still not planning to finish this until the summer; school year's dense.

2. Random Forests on the Kaggle Titanic Dataset - Developing an understanding of decision trees/random forests, and then implementing them in Python. Also learning to manipulate data using Pandas.  
Last worked on: 12/23/2018. Total time: 12h15m

11/9/2018 - Revamped previous efforts on the project, reformatting it for presentation at the UDSC. Next step is still to implement the actual Decision Tree class, but Gini is working. Maybe also categorize other categories if possible?

11/12/2018: 1h - Spent time studying Pandas syntax and useful methods. I'll be presenting this project this Friday at the UDSC and I'll need to better understand Pandas prior to presenting about it. Made some tweaks to the notebook to clean things up and add useful information/resources. I'll need about two hours more to finish the Kaggle Pandas tutorial I'm going through.

11/15/2018: 3h - I spent the time finishing off the end of the notebook as it will be presented tomorrow. I've added methods to calculate entropy and information gain, engineered a few useful features, and cleaned up the mess that was my initial attempt at coding Gini Impurity. I've stopped just short of coding the actual decision tree class. Frankly, I'm unsure exactly how such an implementation's supposed to store the decisions and whatnot. I'll figure that out after presenting.

11/16/2018: 30min - Notebook completed as it will be presented today. Everything including information gain works as expected.

11/25/2018: 3hr - Over the past few days, since Thanksgiving, I've been reading through an in-depth article on all things related to decision trees. It's been a great way to round out my knowledge on the topic so far and I feel like I'm really getting these concepts finally in a comprehensive way. I've gone through a bunch and hope to finish soon before coding these things out. Titanic's a good start but we should test our code on other datasets as well, once we're there.

12/17/2018: 90min - Continuing in the article, this time also reading some textbooks on cross-validation. I also read through the entire notebook and reworded things that weren't ideal. Also covered random forests today; only a bit left to cover.

12/23/2018: 45min - Finished the intial article, moving into academic sources. First part has been on the ID3 algorithm. Apparently gain ratio's better than information gain; who knew? This is formalizing the concepts I already covered, so it's a good path. Probably three days left or fewer until I start coding these up. I should cut off at that point, I think.

3. Gentrification Analysis using Neural Networks/Data Science.  
Last worked on: 11/3/2018. Total time: 5 hours

10/19/2018: 1h - I began by setting up this document before beginning some background research into the causes and effects of gentrification. Also sent out messages to a few sources asking for any considerations I should make in order to remain socially conscious of any broad pictures I might otherwise fail to consider. Seems like an interesting topic with a ton of possible avenues for exploration.

10/22/2018: 1h - Another hour on gentrification, this time finishing the first overview article and beginning another on one approach which used Yelp reviews to quantify gentrification. There's certainly research related to what I'd like to study here, which is simultaneously promising and daunting because I'll need to differentiate my methods explicitly.

10/23/2018: 1h - Spent time today studying what APIs are by following through about half of an hour-long video on Web APIs. I've so far learned the meaning of and the basic processes using web APIs as well as a few examples of how they can be used.

10/24/2018: 1h - In my hour today, I finished the API video and read multiple articles on uses of big data on analyzing city dynamics. I've compiled a number of sources on both big data uses relating to cities and some on useful APIs. These two avenues will round out my knowledge on what's been done in this area of study and similarly give me some ideas for the tools already out there regarding API access to datasets/insights. I plan to read through what I've gathered before cutting myself off, considering my options, and beginning to develop my own ideas for the project. That's the path forward.

11/3/2018: 1h - I went through the sources on useful APIs and decided pretty quickly that I'll need to and want to find the APIs relevant to this project on my own; broad API lists aren't very specialized. After this realization, I spent the rest of the hour researching previous methods for clustering neighborhoods. Data Iku has a great example on this, and I'll read through their methods before looking to additional ways I could cluster neighborhoods. My thought process is that the clustering will determine to what degree we can segment and therefore evaluate our final prediction model. We thus need to ensure that the clustering is as accurate and specific as possible.

4. Blocktr[AI]n - A library for Keras models using some variation on Blockchain. Total time: 0 hours
