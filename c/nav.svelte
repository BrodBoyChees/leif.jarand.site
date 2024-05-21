<nav>
    <div class="nav_contianer">
        <a href="/"><p>Heim</p></a>
        <div class="dropdown">
            <p>Sider</p>
            <div>
                <p>Truenas</p>
                <a href="/truenas/innstalasjon" >Instalasjon</a>
                <a href="/truenas/AD" >Active Direcotory</a>
                <a href="/truenas/lagring" >Oppsett av lagringa</a>
                <a href="/truenas/forlatDomene">Forlate domene i Truenas</a>
                <p>Windows server</p>
                <a href="/win-s/polecy" >Polecy</a>
                <p>Docker</p>
                <a href="/docker/phpapace-mysql" >PHP-  apache og mysql server</a>
            </div>
        </div>
    </div>
</nav>

<style>
    nav{
        height: 70px;
        width: 100%;
        display: flex;
        justify-content: center;
        background: #000;
        z-index: 999;
    }
    .nav_contianer{
        height: 100%;
        width: min(100%, 900px);
        display: flex;
        align-items: center;
        padding: 0 10px 0 10px
    }
    nav a{
        text-decoration: none;
        font-family: quicksand, roboto;
        font-size: 18px;
        color: darkgray;
        transition: .2s;
        display: block;
    }
    nav a p:hover, nav a:hover{
        color: yellow;
    }
    nav p{
        color: white;
        font-size: 25px;
        margin-right: 20px;
    }
    .dropdown{
        font-family: quicksand;
        display: flex;
        align-items: center;
        height: 100%;
    }
    .dropdown p{
        margin: 0;
    }
    .dropdown::after{
        content: '';
        display: inline-block;
        background-image: url(https://img.gamehub.community/kvitpil.png);
        height: 20px;
        width: 20px;
        margin-left: 10px;
        background-position: center;
        background-size: cover;
        transition: .1s;
    }
    .dropdown:hover div{
        display: block;
    }
    .dropdown:hover::after{
        transform: rotate(90deg);
    }
    .dropdown div{
        display: none;
        border-radius: 10px;
        border: 1px solid yellow;
        background: #222;
        position: absolute;
        top: 60px;
        margin-left: -10px;
        padding: 10px;
        width: max-content;
        box-shadow: 0 0 10px rgba(184, 174, 46, 0.253);
    }
</style>