<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
    <style>
        divcontent {
            width: 80vw;
            height: 80vh;
            display: table-cell;
            vertical-align: middle;
            word-break: break-all;

        }

        img {
            max-width: 100%;
            height: auto;
            max-height: 100%;
        }
    </style>


</head>


<body background={% block backgroundUrl %}{% endblock %}>

<div>

    <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js"
            integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n"
            crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js"
            integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo"
            crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js"
            integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6"
            crossorigin="anonymous"></script>

    <div class="navbar navbar-expand-lg navbar-dark bg-dark">  <!--  navbar navbar-expand-lg navbar-light bg-light  -->
        <div class="container">
            <a class="navbar-brand" href="/index">Form</a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
                    aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav mr-auto">


                </ul>
                <div class="navbar-nav">

                    <r3 class="nav-item">
                        <a class="nav-link" href="/about">about</a>
                    </r3>

                    {% if user.is_superuser %}
                        <r3>
                            <li class="nav-item">
                                <a class="nav-link" href="/create">Post</a>
                            </li>
                        </r3>
                    {% endif %}
                    <li class="nav-item dropdown">


                        {% if user.is_authenticated %}


                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                               data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                {{ user.username }}
                            </a>
                            <div class="dropdown-menu" aria-labelledby="navbarDropdown">

                                {% if user.is_superuser %}
                                    <a class="dropdown-item" href="/admin/">Datebase Admin</a>
                                    <a class="dropdown-item" href="/adminp/">Admin</a>
                                {% endif %}
                                <a class="dropdown-item" href="/profile/edit">Profile Edit</a>
                                <div class="dropdown-divider"></div>
                                <a class="dropdown-item" href="/logout">Log out</a>
                            </div>
                            </li>

                        {% else %}

                            <r3 class="nav-item">
                                <a class="nav-link" href="/signup">Sign up</a>
                            </r3>

                            <li class="nav-item">
                                <a class="nav-link" href="/login/">Log in</a>
                            </li>

                        {% endif %}


                </div>
            </div>
        </div>
    </div>

    <br>
    <br>

    <div class="container">
        {% block content %}

        {% endblock %}

    </div>
</div>

</body>

</html>

<h1 align="center">Hello ,Bloodnighttw is here 👋</h1>



<p>&nbsp;&nbsp;&nbsp;&nbsp; I'm a 18 years old senior high school student.My journey on programing isn't long,in fact,I started learning coding on freshman year of senior high school,but after learning ,I know that this will be the way I will choose. I will keep learing forward,until someday nothing could let me learn.</p>

<h1 align="center">My works👋</h1>

<div align="center">

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=bloodnighttw&repo=dotfile)](https://github.com/bloodnighttw/dotfile)
[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=bloodnighttw&repo=Programing-Practice)](https://github.com/bloodnighttw/FileForm)

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=bloodnighttw&repo=DCBot-codeChanger)](https://github.com/bloodnighttw/DCBot-codeChanger)
[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=bloodnighttw&repo=FileForm)](https://github.com/bloodnighttw/FileForm)
</div>

<p align="center">
  <img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=bloodnighttw&hide=javascript,css,html&layout=compact" />
</p>

- I'm EDM Lover.
- Also,I'm Vim Lover,and I use Arch,btw.
![](My-Desktop.png)
