<template>
    <div class="rodapeforget">
        <div class="rodape">
            <div class="left">
                <div class="brand">
                    <a href="#">
                    </a>
                </div>
                <div class="agency">
                    <h1>braflix</h1>
                    <h3>Os melhores filmes estão aqui</h3>
                </div>
            </div>
            <div class="right">
                <div class="socialmedia">
                    <ul>
                        <li>
                            <img src="../img/60580.png" style="filter: invert(100%);">
                        </li>
                        <li>
                            <img src="../img/logo-instagram-png-sem-fundo16.png"
                                style="filter: invert(100%); width: 30px;">
                        </li>
                    </ul>
                </div>
                <div class="agencycontact">
                    <a href="#">
                        <span>Nossas redes sociais</span>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>
<style>
.rodapeforget {
    background-color: #0a0a1270;
    bottom: 0;
    width: 100%;
}

.rodape {
    justify-content: space-between;
    align-items: center;
    padding: 17px;
    display: flex;
    flex-direction: row;
    color: #fff;
    margin: 0 24px;
    margin-right: 120px;
    margin-left: 80px;
    margin-top: 7%;
}

.left {
    display: flex;
}

.logofbi {
    padding: 0px 14px;
    width: 80px;
    height: 80px;
}

.agency {
    display: flex;
    flex-direction: row;
    align-items: center;
    margin: -7px 0 0 0;
}

.agency h1 {
    font-size: 3.9em;
    font-weight: 600;
    font-family: "Arial Black", sans-serif, Arial, Helvetica;
    text-shadow: 0 4px 3px rgb(0 0 0 / 40%), 0 8px 13px rgb(0 0 0 / 10%), 0 18px 23px rgb(0 0 0 / 10%);
    margin: 1px 0 0;
    color: #fff;
}

.agency h3 {
    width: 10.1em;
    letter-spacing: 1px;
    font-weight: 300;
    line-height: 1.1em;
    margin: 4px 0 0 20px;
    text-shadow: 0 4px 3px rgb(0 0 0 / 40%), 0 8px 13px rgb(0 0 0 / 10%), 0 18px 23px rgb(0 0 0 / 10%);
    font-family: Arial, Helvetica, sans-serif;
}

.socialmedia img {
    width: 25px;
    list-style-type: none;
    text-decoration: none;
    padding: 0 10px;
}

ul {
    justify-content: center;
    align-items: center;
    list-style-type: none;
    display: flex;
}

.rigth {
    color: #fff;
}

.agencycontact span {
    text-decoration: none;
    color: rgb(185, 185, 185);
}
</style>