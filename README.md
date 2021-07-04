body {
    margin: 0;
    font-family: 'Roboto', sans-serif;

    font-size: 15px;
    line-height: 1.6;
    color: rgb(207, 205, 223)
}

*,
 :before,
 :after {
    box-sizing: border-box;
}

h1, h2, h3, h4, h5, h6 {
    margin: 0;
}


/*Container*/
.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
}
/*Intro*/
.intro {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    height: 100vh;

    background: url("../intro.jpg") center no-repeat;
    -webkit-background-size: cover;
    background-size: cover;
}

.intro_inner {
    width: 100%;
    max-width: 880;
    margin: 0 auto;
    text-align: center;
}

.intro_title {
    color: aqua;
    font-size: 150px;
    font-weight: 700;
    text-transform: uppercase;
    text-align: center;
    line-height: 1;
}
.intro_title:after{
    content: "";
    display: block;
    width: 60px;
    height: 3px;
    margin: 60px auto;

    background-color: aqua;
}

.intro_suptitle {
    margin-bottom: 20px;
    font-size: 72px;
    color: aqua;
    font-family:'Nothing You Could Do', cursive;
    text-align: center;
}

/*Header*/
.header {
    width: 100%;
    padding-top: 30px;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
}

/*логотип слево, навигацы слево*/
.header_inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.header_logo {
    font-size: 30px;
    font-weight: 700;
    color:rgb(221, 221, 221);
}
/*Nav*/
.nav{
    font-size: 14px;
    text-transform: uppercase;
}
.nav_link {
    display: inline-block;
    vertical-align: top;
    margin:0 10px;
    position: relative;
    color: #cccbd1;
    text-decoration: none;
    transition: color .1s linear;
}
.nav_link:after {
    content: "";
    display: block;
    width: 100%;
    height: 3px;
    opacity: 0;
    background-color: #fce38a;
    position: absolute;
    top: 100%;
    left: 0;
    z-index: 1;

    transition: opacity .1s linear;
}
.nav_link:hover {
    color:#fce38a;

}
.nav_link:hover:after {
    opacity: 1;
}
/*Button*/
.btn {
    display: inline-block;
    vertical-align: top;
    
    padding: 8px  30px;
    border: 3px solid #fff;
    font-size: 14px;
    font-weight: 700;
    color: aqua;
    text-transform: uppercase;
    text-decoration: none;
    transition: background .3s linear, color .1s;
}
.btn:hover {
    background-color: #fce38a;
    color: #333;
}
