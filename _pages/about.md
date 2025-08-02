---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I'm a Staff Research Scientist and Tech Lead at Google Research, where I build factually grounded Large Language Models. My focus is on making Gemini both more knowledgeable and less prone to hallucinations. My research spans the full development cycle of LLMs, from designing pre-training strategies to reinforcement learning techniques that help models better distinguish fact from fiction.

I'm fascinated with a fundamental question: how do language models actually 'know' things? My research interests center on how LLMs acquire, represent, and apply knowledge to reason about the world. I'm particularly interested in the mechanisms by which they internalize factual information during pre-training and how that knowledge can be reliably extracted to enable reasoning.

I completed a PhD in Natural Language Processing at Tel Aviv University, supported by a [Google PhD Fellowship](https://ai.googleblog.com/2018/04/announcing-2018-google-phd-fellows-for.html){:target="_blank" rel="noopener noreferrer" style="color: forestgreen; text-decoration: none;"}. My doctoral research, as well as my three internships at Google, focused on reasoning over structured data. Prior to my PhD, I was a Research Staff Member at IBM Research, where I worked on deep learning for language understanding. My research has been recognized with best paper awards at [INLG](https://aclanthology.org/W17-3541.pdf){:target="_blank" rel="noopener noreferrer" style="color: forestgreen; text-decoration: none;"} and [NAACL](https://arxiv.org/pdf/1811.00937){:target="_blank" rel="noopener noreferrer" style="color: forestgreen; text-decoration: none;"}.

Feel free to reach out if you are interested in collaborating!

## 📜 Publications

---
<style type="text/css">
  .tg  {border-collapse:collapse;border-spacing:0;}
  .tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px; overflow:hidden;padding:10px 5px;word-break:normal;}
  .tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px; font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
  .tg .tg-oe15{background-color:#ffffff;border-color:#ffffff;text-align:left;vertical-align:top}
  .tg .tg-wk8r{background-color:#ffffff;border-color:#ffffff;text-align:center;vertical-align:top}
</style>

<table class="tg">
  <tbody>
    {% for pub in site.data.publications %}
    <tr>
      <td class="tg-wk8r"><strong>{{ pub.venue }}</strong></td>
      <td class="tg-oe15">
        <strong>{{ pub.title }}</strong>
        
        {% if pub.star %}
          <img src="{{ "/images/trophy.png" | relative_url }}" alt="Star" style="width: auto; height: 18px;"/>
        {% endif %}

        {% if pub.award %}
          <span style="color:#800000;">{{ pub.award }}</span>
        {% endif %}

        {% if pub.media %}
          <span style="color:#800000;">{{ pub.media }}</span>
        {% endif %}

        <br>{{ pub.authors }}
        <span style="display: block; margin-bottom: -13px;"></span> <br> 
        
        <a href="{{ pub.pdf }}" target="_blank" rel="noopener noreferrer">
          <img src="https://img.shields.io/badge/Paper-80000f" alt="PDF" style="width: auto; height: 20px;"/>
        </a>
        
        {% if pub.github %}
        <a href="{{ pub.github }}" target="_blank" rel="noopener noreferrer">
          <img src="https://img.shields.io/badge/Code-004f80" alt="GitHub Repository" style="width: auto; height: 20px;"/>
        </a>
        {% endif %}

        {% if pub.project %}
        <a href="{{ pub.project }}" target="_blank" rel="noopener noreferrer">
          <img src="https://img.shields.io/badge/Website-228B22" alt="Project page" style="width: auto; height: 20px;"/>
        </a>
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
