## Robotics Diversity Reading List

The diversity of researchers in academia, and academic robotics specifically, is much lower than it should be. We hope that this reading list will in some small way help to overcome the systemic dynamics that have lead to this inbalance. There are two ways that this list may help: 
First, we want to increase the impact of these researchers by highlighting their research projects and advertising some of their interesting papers. We built this list to help people find knowledgeable experts for panels, possible advisors for graduate school, good citations on a given topic, and discover new exciting ideas. 
In addition to increasing the impact of these researchers, we also wanted to provide role models for prospective graduate students. Whether browsing this list online, seeing a researcher on a panel, or reading one of their papers as a class assignment it is important for all students to see diversity in academia. 

Who is this list for? We started to build this list for our own labs and classes, to increase the diversity of the researchers we discuss and cite. We hope that it can also be useful for others in the community, especially:
* Undergraduate students looking for possible graduate school mentors.
* Paper authors looking for a citation on a given topic.
* Workshop or panel organizers looking for experts in the field.
* Instructors building a reading list for a class syllabus.
* Everyone in the community who would like to learn more about new cutting edge research in different areas of robotics.

The focus we have chosen for this list is black professors in the US researching robotics and related fields. While there are many groups that are underrepresented in robotics, there is a particularly long and persistent history of suppression of black Americans in the US. There are also many great roboticists in industry, and many great academics outside of robotics, that should also be celebrated. Over time we may grow this list to support and celebrate a broader group of researchers.


{% assign items = site.people | sort: 'last_name' %}
{% for person in items %}
<div class="person">
  <table border="0px">
    <tr>
    <td><img src="{{ person.image  }}"></td>
    <td>
      <h2>{{ person.first_name }} {{ person.last_name }}</h2>
      <p><a href="{{ person.website }}">{{ person.title }}</a>, {{  person.school  }} </p>
      <p>{{ person.content | markdownify }}</p>
    </td>
    </tr>
  </table>
</div>
{% endfor %}
