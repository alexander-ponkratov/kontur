<template>
    <header class="header">
        <nav id="main-navbar" class="navbar navbar-default navbar-fixed-top">
            <div class="container navbar-container">
                <div class="navbar-header">
                    <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar"
                        aria-expanded="false" aria-controls="navbar">
                        <span class="sr-only">Toggle navigation</span>
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                    </button>
                    <a class="navbar-brand" href="#">Logo</a>
                </div>
                <div id="navbar" class="navbar-collapse collapse">
                    <ul class="nav navbar-nav navbar-right">
                        <li><a href="#">Home</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#portfolio">Portfolio</a></li>
                        <li><a href="#contact">Contact</a></li>
                        <li><a href="#blog">Blog</a></li>
                    </ul>
                </div>
                <div class="top-social">
                    <ul id="top-social-menu">
                        <li><a href="#"><i class="fa fa-twitter"></i></a></li>
                        <li><a href="#"><i class="fa fa-facebook"></i></a></li>
                        <li><a href="#">Register</a></li>
                        <li><a href="#">Careers</a></li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>


<!-- component script -->
<script>
export default {
    /* passed props */
    props: {
    },
    /*     data: () => ({
        }), */
    /* js code */
    mounted() {
        $(window).scroll(function () {
            var sc = $(window).scrollTop()
            if (sc > 150) {
                $("#main-navbar").addClass("navbar-scroll")
            }
            else {
                $("#main-navbar").removeClass("navbar-scroll")
            }
        });
    },
    methods: {
    }
}
</script>

<!-- component style -->
<style scoped lang="scss">
/* # General
================================ */

body {
    font-family: "Open Sans", Helvetica, sans-serif;
}

/* # Header, Main Menu
================================ */

.navbar {
    opacity: 0.8;
    margin-bottom: 0;
    background-color: #fff;
    transition: all 0.2s ease-out;
}

.navbar-container {
    position: relative;
}

.navbar .navbar-nav li a {
    font-size: 14px;
    text-transform: uppercase;
    color: #2E1C05;
    transition: all 0.2s ease-out;
}

.navbar-brand {
    font-size: 25px;
    transition: all 0.2s ease-out;
}

.navbar-scroll {
    opacity: 1;
}

#top-social-menu {
    display: none;
}


@media (min-width: 768px) {
    .navbar {
        height: 120px;
    }

    .navbar-nav>li>a {
        padding: 0;
        margin-top: 35px;
        margin-left: 50px;
        line-height: 70px;
    }

    .navbar-brand {
        font-size: 28px;
        padding: 0;
        height: 120px;
        line-height: 120px;
    }

    #top-social-menu {
        display: initial;
    }

    /* Navbar when scrolled */

    .navbar-scroll {
        height: 70px;
    }

    .navbar-scroll #top-social-menu {
        display: none;
        transition: all 0.2s ease-out;
    }

    .navbar-scroll .navbar-brand {
        height: 70px;
        line-height: 70px;
    }

    .navbar-scroll .navbar-nav>li>a {
        opacity: 1;
        padding: 0;
        margin-top: 0;
    }
}

/* # Hover Link Effect
================================ */
@media (min-width: 768px) {
    .navbar-nav>li>a::after {
        position: absolute;
        top: 80%;
        left: 0;
        width: 100%;
        height: 1px;
        background: #2E1C05;
        content: '';
        opacity: 0;
        transition: height 0.3s, opacity 0.3s, transform 0.3s;
        transform: translateY(-10px);
    }

    .navbar-nav>li>a:hover::after,
    .navbar-nav>li>a:focus::after {
        height: 2px;
        opacity: 1;
        transform: translateY(0px);
    }
}

/* # Social menu
================================ */

#top-social-menu {
    position: absolute;
    top: 7px;
    right: 0;
    font-size: 12px;
    z-index: 101;
    padding-right: 0px;
    list-style: none;
    color: #2E1C05;
    transition: all 0.2s ease-out;
}

#top-social-menu li {
    float: left;
    padding: 10px 15px;
}

#top-social-menu li:last-child {
    padding-right: 0;
}

#top-social-menu li a {
    text-decoration: none;
    color: #2E1C05;
}

#top-social-menu li a:hover {
    text-decoration: none;
    color: #543A1A;
}

#top-social-menu i {
    font-size: 16px;

    transition: all 0.2s ease-in;
}

#top-social-menu i:hover {
    text-decoration: none;
    color: #543A1A;
}

/* # Section Full Width Image
================================ */

.full-width-img {
    background: url('http://res.cloudinary.com/do5ht5y0y/image/upload/v1501322753/bg-cp-header_zps4ghnoxc7_zx2ayd.jpg') no-repeat center center;
    background-size: cover;
    text-align: center;
    padding-top: 100px;
    height: 450px;
    color: #fff;
}

.box {
    background: rgba(0, 0, 0, 0.4);
    border: 3px solid #000;
    color: #fff;
    text-align: center;
    margin-top: 10px;
    padding: 10px 20px;
}

.subheading-text {
    list-style: none;
    font-size: 35px;
    line-height: 50px;
}

@media (min-width: 768px) {

    .full-width-img {
        padding-top: 110px;
        height: 1000px;
    }

    .subheading-text {
        font-size: 50px;
        line-height: 70px;
    }

    .box {
        margin-top: 100px;
        padding: 80px 20px;
    }
}

/* # Section Black, White
================================ */

.section-black,
.section-white {
    padding: 50px 0;
    color: #fff;
    line-height: 1.7;
}

.section-black h3,
.section-white h3 {
    margin-bottom: 60px;
}

.section-black p,
.section-white p {
    margin-bottom: 60px;
}

.section-black {
    background: linear-gradient(#363437, #121112);
}

.section-white {
    background: linear-gradient(#ffffff, #f3f3f3);
    color: #0e0d0e;
}
</style>