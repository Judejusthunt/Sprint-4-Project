# Sprint-4-Project
This is the Repository that will be used for my Sprint 4 Project in the Triple Ten Data Science Program.


<section class="theory-viewer prisma prisma_theme_light big-theory lesson__homework-theory"><section class="theory-viewer__blocking-layout-block theory-viewer__block theory-viewer__block_type_vertical-layout theory-viewer__block_layout"><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h1>Project Description</h1><div class="paragraph">Congratulations! You’ve completed the section on Software Development Tools. Now it’s time to apply the knowledge and skills you’ve acquired to a project: building and deploying a web application dashboard to a cloud service.</div><div class="paragraph">Once you’ve finished the project remember to send your work to the project reviewer for assessment. They’ll give you feedback within 24 hours. Use the feedback to make changes, then send the new version back to the project reviewer.</div><div class="paragraph">You might get further feedback on the new version. This is completely normal. It’s not uncommon to go through several cycles of feedback and revision.</div><div class="paragraph">Your project will be considered complete once the project reviewer approves it.</div></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h1>Project description</h1><div class="paragraph">The focus of this project is to provide you with additional practice with common software engineering tasks. These will augment and complement your data skills, and make you a more attractive job candidate to potential employers. </div><div class="paragraph">The tasks are: creating and managing python virtual environments, developing a web application, and deploying it to a cloud service that will make it accessible to the public.</div><div class="paragraph">In this project, we are providing you with a dataset you are already familiar with: a dataset of car sales advertisements. However, in this project, the focus will not be on the dataset or the analysis, and thus you are free, and even encouraged, to choose any dataset that you want.</div><div class="paragraph">The project is split into several steps that replicate the process described in <a href="https://www.practicum.blog/posts/deploying-data-science-web-apps-to-the-cloud" target="_blank">one of our blog posts</a>.</div><div class="paragraph"><div class="iframe-wrapper"><iframe allowfullscreen="" src="https://www.youtube.com/embed/bna15Zj6jUI"></iframe></div>
Demo of the web application you’ll build in this project</div></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h1>Instructions for completing the project</h1></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h3>Step 1. Project Prerequisites</h3><ol start="1"><li>Create an account on <a href="http://github.com" target="_blank">github.com</a></li><li>Create a new git repository with a <code class="code-inline code-inline_theme_light">README.md</code> file and a <code class="code-inline code-inline_theme_light">.gitignore</code> file (choose a Python template).</li><li>Install at least the following packages: <code class="code-inline code-inline_theme_light">pandas</code>, <code class="code-inline code-inline_theme_light">streamlit</code>, <code class="code-inline code-inline_theme_light">plotly-express</code>. Feel free to install more packages if you want to implement additional features in your web app.</li><li>Create an account on <a href="http://render.com" target="_blank">render.com</a>, link it to your GitHub account</li><li><a href="https://code.visualstudio.com/download" target="_blank">Install VS Code</a>, load the project directory and set the Python interpreter to the one used by the virtual environment</li></ol></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h3>Step 2. Download <strong>the data file</strong></h3><ol start="1"><li><a href="https://practicum-content.s3.us-west-1.amazonaws.com/datasets/vehicles_us.csv" target="_blank">Download the car advertisement dataset</a> (<code class="code-inline code-inline_theme_light">vehicles_us.csv</code>) or find your own dataset in a CSV format</li><li>Place the dataset in the root directory of the project</li></ol><div class="paragraph">Note: for project ideas and inspiration, check out <a href="https://www.youtube.com/watch?v=JwSS70SZdyM" target="_blank">this video</a>.</div></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h3>Step 3. Exploratory Data Analysis</h3><ol start="1"><li>Create an <code class="code-inline code-inline_theme_light">EDA.ipynb</code> Jupyter notebook in VS Code</li><li>Save the notebook in the <code class="code-inline code-inline_theme_light">notebooks</code> directory of your project</li><li>Perform some basic exploratory analysis of the dataset in the notebook</li><li>Create a couple of histograms and scatterplots using <code class="code-inline code-inline_theme_light">plotly-express</code> library</li></ol><div class="paragraph">Note: </div><ul><li>if you are using the car advertisement dataset, it won’t be sufficient to simply recreate the plots described in the blog post to complete the project. You’ll have to get creative and come up with your own plots and histograms.</li><li>it’s often very convenient to experiment with data visualizations in Jupyter, and then copy-paste code into a web application file later</li></ul></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h3>Step 4. Develop the web application dashboard</h3><ol start="1"><li>Create an <code class="code-inline code-inline_theme_light">app.py</code> file in the root of the project’s directory</li><li>Import <code class="code-inline code-inline_theme_light">streamlit</code>, <code class="code-inline code-inline_theme_light">pandas</code> and <code class="code-inline code-inline_theme_light">plotly_express</code></li><li>Read the dataset’s CSV file into a DataFrame</li><li>Create and/or copy from the Jupyter notebook:
 <ul><li>at least one <a href="https://docs.streamlit.io/library/api-reference/text/st.header" target="_blank"><code class="code-inline code-inline_theme_light">st.header</code></a> with text</li><li>at least one <code class="code-inline code-inline_theme_light">plotly-express</code> histogram using <a href="https://docs.streamlit.io/library/api-reference/write-magic/st.write" target="_blank"><code class="code-inline code-inline_theme_light">st.write</code></a> or <a href="https://docs.streamlit.io/library/api-reference/charts/st.plotly_chart" target="_blank"><code class="code-inline code-inline_theme_light">st.plotly_chart</code></a></li><li>at least one <code class="code-inline code-inline_theme_light">plotly-express</code> scatter plot using <a href="https://docs.streamlit.io/library/api-reference/write-magic/st.write" target="_blank"><code class="code-inline code-inline_theme_light">st.write</code></a> or <a href="https://docs.streamlit.io/library/api-reference/charts/st.plotly_chart" target="_blank"><code class="code-inline code-inline_theme_light">st.plotly_chart</code></a></li><li>at least one checkbox using <a href="https://docs.streamlit.io/library/api-reference/widgets/st.checkbox" target="_blank"><code class="code-inline code-inline_theme_light">st.checkbox</code></a> that changes the behavior of any of the above components</li></ul></li><li>Don’t forget to update the <code class="code-inline code-inline_theme_light">README</code> file when you are done. It should contain some basic description of the project and instructions on how other people could launch your project on their local machine if they wanted to.</li><li><strong>IMPORTANT: Replit will fail to build your project unless all project files are present in your GitHub repository</strong>. Therefore, you must commit and push file changes to your repository when you’re done with your work.</li></ol><div class="paragraph">Notes: </div><ul><li>as you develop your application by adding a new Streamlit component, you can run <code class="code-inline code-inline_theme_light">streamlit run app.py</code> command from the terminal to see what the result looks like</li><li>as you reach some milestones in the application development (e.g. you add a working component and the application runs without errors), it’s a good practice to commit and push your work to a remote repository on GitHub. So don’t forget to write a meaningful commit message!</li></ul></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h3>Step 5. Deploy the final version of the application to Render</h3><ol start="1"><li>To make streamlit compatible with render, add a streamlit configuration file to your git repository at <code class="code-inline code-inline_theme_light">.streamlit/config.toml</code> with the following content:</li></ol><div class="toml code-block code-block_theme_light"><div class="code-block__tools"><button class="code-block__clipboard" type="button">Copy code</button><span class="code-block__lang">TOML</span></div><div class="scrollable-default scrollable scrollable_theme_light code-block__scrollable prisma prisma_theme_light"><div></div><div class="scrollable__content-wrapper"><div class="scrollbar-remover scrollable__content-container" style="--scroll-bar-width: 18px; --scroll-bar-height: 18px;"><div class="scrollable__content"><pre class="code-block__code-wrapper"><code class="code-block__code toml">[server]
headless = true
port = 10000

[browser]
serverAddress = "0.0.0.0"
serverPort = 10000 </code></pre><div></div></div></div></div><section class="scrollbar-default scrollbar scrollbar_vertical scrollbar_hidden scrollable__scrollbar scrollable__scrollbar_type_vertical" size="1" style="--scrollbar-offset-size: 177px; --scrollbar-control-size: 177px; --scrollbar-control-container-size: 100%; --scrollbar-scale: 1; --scrollbar-control-offset: 0;"><div class="scrollbar__control-container"><div class="scrollbar__control"><div class="scrollbar__control-line"></div></div></div></section><section class="scrollbar-default scrollbar scrollbar_horizontal scrollbar_hidden scrollable__scrollbar scrollable__scrollbar_type_horizontal" size="1" style="--scrollbar-offset-size: 688px; --scrollbar-control-size: 688px; --scrollbar-control-container-size: 100%; --scrollbar-scale: 1; --scrollbar-control-offset: 0;"><div class="scrollbar__control-container"><div class="scrollbar__control"><div class="scrollbar__control-line"></div></div></div></section></div></div><div class="paragraph">It’ll tell Render to look in the right place to listen to your streamlit app when hosting it on its servers.</div><ol start="2"><li>Open your account on <a href="http://render.com" target="_blank">render.com</a> and create a new web service:</li></ol><div class="paragraph paragraph_has-one-child"><div class="downloadable-image prisma prisma_theme_light"><button class="prisma-button prisma-button_icon-placement_left prisma-button_position-in-group_none prisma-button_size_s prisma-button_view_ghost downloadable-image__button"><span class="prisma-button__content"><span class="prisma-button__text"><span class="prisma-button__label"><svg class="prisma-icon prisma-icon_type_arrows-download-24 downloadable-image__icon" width="24" height="24" viewBox="0 0 24 24" fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 3C11.45 3 11 3.45 11 4V10.9219C11 11.6763 11.0854 12.4276 11.254 13.1613L11.0483 13.3684L10.8331 13.0242C10.4323 12.3835 9.96022 11.7902 9.42583 11.2558L8.46 10.29C8.07 9.89999 7.44 9.89999 7.05 10.29C6.66 10.68 6.66 11.32 7.05 11.71L10.9404 15.5926C11.526 16.1769 12.474 16.1769 13.0596 15.5926L16.95 11.71C17.34 11.32 17.34 10.68 16.95 10.29C16.56 9.89999 15.93 9.89999 15.54 10.29L14.5742 11.2558C14.0398 11.7902 13.5677 12.3835 13.1669 13.0242L12.9517 13.3684L12.746 13.1613C12.9146 12.4276 13 11.6763 13 10.9219V4C13 3.45 12.55 3 12 3ZM7 19C6.44772 19 6 19.4477 6 20C6 20.5523 6.44772 21 7 21H17C17.5523 21 18 20.5523 18 20C18 19.4477 17.5523 19 17 19H7Z" fill="currentColor" fill-opacity="0.85"></path></svg></span></span></span></button><img src="https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/SDT/sdt-pr-v2-01.png?etag=3b3aeba0f3b456d27fc7fc083d123bcd" alt="image" class="image image_expandable"></div></div><ol start="3"><li>Create a new web service linked to your Github repository:</li></ol><div class="paragraph paragraph_has-one-child"><div class="downloadable-image prisma prisma_theme_light"><button class="prisma-button prisma-button_icon-placement_left prisma-button_position-in-group_none prisma-button_size_s prisma-button_view_ghost downloadable-image__button"><span class="prisma-button__content"><span class="prisma-button__text"><span class="prisma-button__label"><svg class="prisma-icon prisma-icon_type_arrows-download-24 downloadable-image__icon" width="24" height="24" viewBox="0 0 24 24" fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 3C11.45 3 11 3.45 11 4V10.9219C11 11.6763 11.0854 12.4276 11.254 13.1613L11.0483 13.3684L10.8331 13.0242C10.4323 12.3835 9.96022 11.7902 9.42583 11.2558L8.46 10.29C8.07 9.89999 7.44 9.89999 7.05 10.29C6.66 10.68 6.66 11.32 7.05 11.71L10.9404 15.5926C11.526 16.1769 12.474 16.1769 13.0596 15.5926L16.95 11.71C17.34 11.32 17.34 10.68 16.95 10.29C16.56 9.89999 15.93 9.89999 15.54 10.29L14.5742 11.2558C14.0398 11.7902 13.5677 12.3835 13.1669 13.0242L12.9517 13.3684L12.746 13.1613C12.9146 12.4276 13 11.6763 13 10.9219V4C13 3.45 12.55 3 12 3ZM7 19C6.44772 19 6 19.4477 6 20C6 20.5523 6.44772 21 7 21H17C17.5523 21 18 20.5523 18 20C18 19.4477 17.5523 19 17 19H7Z" fill="currentColor" fill-opacity="0.85"></path></svg></span></span></span></button><img src="https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/SDT/sdt-pr-v2-02.png?etag=f516fc54966d96fe5a72277d4b644416" alt="image" class="image image_expandable"></div></div><ol start="4"><li>Configure the new Render web service. To your <strong>Build Command,</strong> add</li></ol><div class="bash code-block code-block_theme_light"><div class="code-block__tools"><button class="code-block__clipboard" type="button">Copy code</button><span class="code-block__lang">BASH</span></div><div class="scrollable-default scrollable scrollable_theme_light code-block__scrollable prisma prisma_theme_light"><div></div><div class="scrollable__content-wrapper"><div class="scrollbar-remover scrollable__content-container" style="--scroll-bar-width: 18px; --scroll-bar-height: 18px;"><div class="scrollable__content"><pre class="code-block__code-wrapper"><code class="code-block__code bash">pip install streamlit &amp; pip install -r requirements.txt </code></pre><div></div></div></div></div><section class="scrollbar-default scrollbar scrollbar_vertical scrollbar_hidden scrollable__scrollbar scrollable__scrollbar_type_vertical" size="1" style="--scrollbar-offset-size: 34px; --scrollbar-control-size: 34px; --scrollbar-control-container-size: 100%; --scrollbar-scale: 1; --scrollbar-control-offset: 0;"><div class="scrollbar__control-container"><div class="scrollbar__control"><div class="scrollbar__control-line"></div></div></div></section><section class="scrollbar-default scrollbar scrollbar_horizontal scrollbar_hidden scrollable__scrollbar scrollable__scrollbar_type_horizontal" size="1" style="--scrollbar-offset-size: 688px; --scrollbar-control-size: 688px; --scrollbar-control-container-size: 100%; --scrollbar-scale: 1; --scrollbar-control-offset: 0;"><div class="scrollbar__control-container"><div class="scrollbar__control"><div class="scrollbar__control-line"></div></div></div></section></div></div><div class="paragraph">To your <strong>Start Command,</strong> add: <code class="code-inline code-inline_theme_light">streamlit run app.py</code>. It should look like this:</div><div class="paragraph paragraph_has-one-child"><div class="downloadable-image prisma prisma_theme_light"><button class="prisma-button prisma-button_icon-placement_left prisma-button_position-in-group_none prisma-button_size_s prisma-button_view_ghost downloadable-image__button"><span class="prisma-button__content"><span class="prisma-button__text"><span class="prisma-button__label"><svg class="prisma-icon prisma-icon_type_arrows-download-24 downloadable-image__icon" width="24" height="24" viewBox="0 0 24 24" fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 3C11.45 3 11 3.45 11 4V10.9219C11 11.6763 11.0854 12.4276 11.254 13.1613L11.0483 13.3684L10.8331 13.0242C10.4323 12.3835 9.96022 11.7902 9.42583 11.2558L8.46 10.29C8.07 9.89999 7.44 9.89999 7.05 10.29C6.66 10.68 6.66 11.32 7.05 11.71L10.9404 15.5926C11.526 16.1769 12.474 16.1769 13.0596 15.5926L16.95 11.71C17.34 11.32 17.34 10.68 16.95 10.29C16.56 9.89999 15.93 9.89999 15.54 10.29L14.5742 11.2558C14.0398 11.7902 13.5677 12.3835 13.1669 13.0242L12.9517 13.3684L12.746 13.1613C12.9146 12.4276 13 11.6763 13 10.9219V4C13 3.45 12.55 3 12 3ZM7 19C6.44772 19 6 19.4477 6 20C6 20.5523 6.44772 21 7 21H17C17.5523 21 18 20.5523 18 20C18 19.4477 17.5523 19 17 19H7Z" fill="currentColor" fill-opacity="0.85"></path></svg></span></span></span></button><img src="https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/SDT/sdt-pr-v2-03.png?etag=c7138c0b557822519ce426c802d81ce6" alt="image" class="image image_expandable"></div></div><ol start="5"><li>Deploy to Render, wait for the build to succeed:</li></ol><div class="paragraph paragraph_has-one-child"><div class="downloadable-image prisma prisma_theme_light"><button class="prisma-button prisma-button_icon-placement_left prisma-button_position-in-group_none prisma-button_size_s prisma-button_view_ghost downloadable-image__button"><span class="prisma-button__content"><span class="prisma-button__text"><span class="prisma-button__label"><svg class="prisma-icon prisma-icon_type_arrows-download-24 downloadable-image__icon" width="24" height="24" viewBox="0 0 24 24" fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 3C11.45 3 11 3.45 11 4V10.9219C11 11.6763 11.0854 12.4276 11.254 13.1613L11.0483 13.3684L10.8331 13.0242C10.4323 12.3835 9.96022 11.7902 9.42583 11.2558L8.46 10.29C8.07 9.89999 7.44 9.89999 7.05 10.29C6.66 10.68 6.66 11.32 7.05 11.71L10.9404 15.5926C11.526 16.1769 12.474 16.1769 13.0596 15.5926L16.95 11.71C17.34 11.32 17.34 10.68 16.95 10.29C16.56 9.89999 15.93 9.89999 15.54 10.29L14.5742 11.2558C14.0398 11.7902 13.5677 12.3835 13.1669 13.0242L12.9517 13.3684L12.746 13.1613C12.9146 12.4276 13 11.6763 13 10.9219V4C13 3.45 12.55 3 12 3ZM7 19C6.44772 19 6 19.4477 6 20C6 20.5523 6.44772 21 7 21H17C17.5523 21 18 20.5523 18 20C18 19.4477 17.5523 19 17 19H7Z" fill="currentColor" fill-opacity="0.85"></path></svg></span></span></span></button><img src="https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/SDT/sdt-pr-v2-04.png?etag=8eb12b130758c89a1eab463f96c44a17" alt="image" class="image image_expandable"></div></div><ol start="6"><li>Verify that your application is accessible at the following URL: <code class="code-inline code-inline_theme_light">https://&lt;APP_NAME&gt;.onrender.com/</code></li></ol><div class="paragraph"><strong>Note:</strong> it can take several minutes after a succesful deployment for the app to be available online on a free tier. Also note that apps go “asleep” after being inactive for a few minutes. If so, just load and refresh your app a few times for it to get awoken.</div></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h2>How to submit my project:</h2><div class="paragraph">You’ll need to submit a link to your GitHub repository. Please also add the URL of your app on Render to your project’s <code class="code-inline code-inline_theme_light">README.md</code></div></div></section><section class="theory-viewer__block theory-viewer__block_type_markdown"><div class="Markdown base-markdown base-markdown_with-gallery markdown markdown_size_normal markdown_type_theory full-markdown"><h2>How will my project be evaluated?</h2><div class="paragraph">We've put together some project assessment criteria. Read over them carefully before you make a submission.</div><div class="paragraph">Here’s what project reviewers look for when assessing your project:</div><ul><li>Does the project repository contain at least the following files?</li></ul><div class="code-block code-block_theme_light"><div class="code-block__tools"><button class="code-block__clipboard" type="button">Copy code</button></div><div class="scrollable-default scrollable scrollable_theme_light code-block__scrollable prisma prisma_theme_light"><div></div><div class="scrollable__content-wrapper"><div class="scrollbar-remover scrollable__content-container" style="--scroll-bar-width: 18px; --scroll-bar-height: 18px;"><div class="scrollable__content"><pre class="code-block__code-wrapper"><code class="code-block__code"># The minimal expected project structure
$ tree
.
├── README.md
├── app.py
├── &lt;name_of_your_dataset&gt;.csv
└── notebooks
    └── EDA.ipynb
└── .streamlit
    └── config.toml </code></pre><div></div></div></div></div><section class="scrollbar-default scrollbar scrollbar_vertical scrollable__scrollbar scrollable__scrollbar_type_vertical" style="--scrollbar-offset-size: 232px; --scrollbar-control-size: 216.83076923076925px; --scrollbar-control-container-size: 100%; --scrollbar-scale: 1; --scrollbar-control-offset: 0;"><div class="scrollbar__control-container"><div class="scrollbar__control"><div class="scrollbar__control-line"></div></div></div></section><section class="scrollbar-default scrollbar scrollbar_horizontal scrollbar_hidden scrollable__scrollbar scrollable__scrollbar_type_horizontal" size="1" style="--scrollbar-offset-size: 688px; --scrollbar-control-size: 688px; --scrollbar-control-container-size: 100%; --scrollbar-scale: 1; --scrollbar-control-offset: 0;"><div class="scrollbar__control-container"><div class="scrollbar__control"><div class="scrollbar__control-line"></div></div></div></section></div></div><ul><li>Is the web app accessible via a browser?</li><li>Does the web app contain the following?
  <ul><li>at least one header with text</li><li>at least 1 histogram</li><li>at least 1 scatter plot</li></ul></li></ul></div></section></section></section>


  <b> NOTE:<b> The link to the app on Render is :  https://sprint-4-project-jude-hunt-5.onrender.com
