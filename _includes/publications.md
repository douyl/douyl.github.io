<!-- 
This code generates a list of publications with various details such as title, authors, conference, links, and citation information. It uses a for loop to iterate over the publications data and dynamically generates the HTML markup for each publication.

The publications are displayed in an ordered list (<ol>) with each publication represented as a list item (<li>). The list item contains a row (<div class="pub-row">) with two columns: one for the publication image and abbreviation, and the other for the publication details.

The publication image is displayed using an <img> tag with the source specified by the "link.image" variable. The abbreviation of the conference is displayed as a badge using the <abbr> tag.

The publication details such as title, authors, and conference are displayed within their respective <div> tags.

The links associated with the publication (PDF, code, project page, BibTex) are displayed as buttons using the <a> tag with the appropriate href and target attributes. The buttons are styled using CSS classes.

If there are any additional notes or other information associated with the publication, they are displayed using the <strong> and <i> tags.

If the publication has citation information available, it is displayed within a nested for loop. The citation information includes the title, year, number of citations, and a link to the "Cited By" page.

The code is written in Markdown and is intended to be used in a website or web page to display a list of publications.

-->
<h1 id="publications"></h1>

<h2 style="margin: 30px 0px -15px;">Publications <temp style="font-size:15px;">[</temp><a href="https://scholar.google.com/citations?hl=zh-CN&authuser=1&user=2gXabhsAAAAJ" rel="noopener noreferrer" target="_blank" style="font-size:15px;">Google Scholar</a><temp style="font-size:15px;">]</temp></h2>


<div class="publications">
  <ol class="bibliography">
    <!-- Publication 2 -->
    <li>
      <div class="pub-row">
        <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
          <img src="./assets/img/TeethDreamer.png" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
          <abbr class="badge">MICCAI</abbr>
        </div>
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><a href="https://shanghaitech-impact.github.io/TeethDreamer/" rel="noopener noreferrer" target="_blank">TeethDreamer: 3D Teeth Reconstruction from Five Intra-oral Photographs</a></div>
          <div class="author">Chenfan Xu, Zhentao Liu, Yuan Liu, <strong><u>Yulong Dou</u></strong>, Jiamin Wu, Jiepeng Wang, Minjiao Wang, Dinggang Shen, Zhiming Cui</div>
          <div class="publisher"><em>International Conference on Medical Image Computing and Computer Assisted Intervention (MICCAI), 2024.</em></div>
          <div class="links">
            <a href="https://shanghaitech-impact.github.io/TeethDreamer/" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">Project Page</a>
            <a href="https://papers.miccai.org/miccai-2024/paper/1038_paper.pdf" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">PDF</a>
            <a href="https://github.com/ShanghaiTech-IMPACT/TeethDreamer" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">Code</a>
          </div>
        </div>
      </div>
    </li>
    <!-- Publication 1 -->
    <li>
      <div class="pub-row">
        <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
          <img src="./assets/img/2DToothAlign.png" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
          <abbr class="badge">BMVC</abbr>
        </div>
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><a href="https://proceedings.bmvc2023.org/322/" rel="noopener noreferrer" target="_blank">3D Structure-guided Network for Tooth Alignment in 2D Photograph</a></div>
          <div class="author"><strong><u>Yulong Dou</u></strong>, Lanzhuju Mei, Dinggang Shen, Zhiming Cui</div>
          <div class="publisher"><em>The 34th British Machine Vision Conference (BMVC), 2023.</em></div>
          <div class="links">
            <a href="https://proceedings.bmvc2023.org/322/" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">Project Page</a>
            <a href="https://papers.bmvc2023.org/0322.pdf" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">PDF</a>
            <a href="https://bmvc2022.mpi-inf.mpg.de/BMVC2023/0322_poster.pdf" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">Poster</a>
            <a href="https://github.com/ShanghaiTech-IMPACT/3D-Structure-guided-Network-for-Tooth-Alignment-in-2D-Photograph" class="btn btn-sm z-depth-0" role="button" rel="noopener noreferrer" target="_blank" style="font-size:12px;">Code</a>
          </div>
        </div>
      </div>
    </li>

  </ol>
</div>







<!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->

<!-- 
<div class="publications">
<ol class="bibliography">
{% assign gsDataBaseUrl = 'https://raw.githubusercontent.com/song-chen1/song-chen1.github.io/' %}
{% assign url = gsDataBaseUrl | append: 'google-scholar-stats/gs_data.json' %}
{% for link in site.data.publications.main %}


<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
            <abbr class="badge">{{ link.conference_short }}</abbr>
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
      {% if link.citation %} 
      <strong> <a style="color:#e74d3c; font-weight:600"> • <i class="total_citation_mtl" data-citation="{{ link.citation }}"></i> <i style="color:#e74d3c; font-weight:600"> Citations </i></a></strong>
      <script>
        $(document).ready(function () {
            var gsDataBaseUrl = 'https://raw.githubusercontent.com/song-chen1/song-chen1.github.io/';
            $.getJSON(gsDataBaseUrl + "google-scholar-stats/gs_data.json", function (data) {
                var citationEles = document.getElementsByClassName('total_citation_mtl');
                Array.prototype.forEach.call(citationEles, function(element) {
                    var citationKey = element.getAttribute('data-citation');
                    if (data['publications'][citationKey]) {
                        var numCitations = data['publications'][citationKey]['num_citations'];
                        element.innerHTML = numCitations;
                    } else {
                        element.innerHTML = 'N/A';
                    }
                });
            });
        });
      </script>
      {% endif %}
    </div>
  </div>
</div>

</li>

<br>

{% endfor %} -->