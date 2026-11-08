# novel-genome-analysis-tool

A novel genome analysis tool with promising results on 1 GB of real genomic data.
There's a new v6 version that is fully parallel and beautifully utilises unlimited amount of cores.
Just make sure to leave at least one core free in order to make the computer usable, as the
parallel code is so well optimised it uses 100% all the time! Therefore perfect cooling is required too!

HOW TO RUN IT
In order to launch the program from console, use command "cd" + working directory to get into folder where the software is
Make sure you have Python installed with all of the libraries the software uses.
Run console command with arguments --email "your-email-address" and optional flags --full --extra --ultra or --mega to download and analyse more and more genomes from the data bank
e.g.
python Genome_Sequencing_v5.py --email your@email.com --extra
You should have console output with text data similar to what you see in Output600MB.txt file, then there will be genomic cache folder where all the genomes are downloaded and cached and then there's output folder where graphs and JSON files are stored.
Running with just email without other arguments is instant, --full argument takes a few seconds to complete, --extra takes about 5 minutes and --ultra can easily take an hour to process.
Note that your email is required to pull the genomic data from the official site. No verification is required, it is used to ban certain users if they abuse the server limits and pull data thousand times an hour.
That's also the reason why genomic data is cached, so program won't spam the servers with every run.
Please note the analysis steps that are too computing intensive are trimmed to just the first 200 thousand basepairs. In order to run the full analysis just search for every mention
of number 200 000 in the code and change it to let's say 2 billion for a full analysis, although this might take several hours with ease.
Please note that version 6.1 is well tested, while version 6.3GPU is GPU accelerated and provides deeper insights, but it might easily cause trouble.
