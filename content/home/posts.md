+++
# Recent Posts widget.
# This widget displays recent posts from `content/post/`.
widget = "posts"
active = true
date = "2016-04-20T00:00:00"

title = "Work Experience"
subtitle = ""

# Order that this section will appear in.
weight = 40

# List your qualifications (such as academic degrees).
[[education.courses]]
  course = "M.S. in Computer Science"
  institution = "North Carolina State University"
  year = 2017


[[education.courses]]
  course = "B.E. in Computer Science"
  institution = "Jawaharlal Nehru Engineering College"
  year = 2011
       {{ with $page.Params.education }}
      <div class="col-sm-7">
        <h3>{{ i18n "education" | markdownify }}</h3>
        <ul class="ul-edu fa-ul">
          {{ range .courses }}
          <li>
            <i class="fa-li fa fa-graduation-cap"></i>
            <div class="description">
              <p class="course">{{ .course }}{{ with .year }}, {{ . }}{{ end }}</p>
              <p class="institution">{{ .institution }}</p>
            </div>
          </li>
          {{ end }}
        </ul>
      </div>
      {{ end }}

+++

