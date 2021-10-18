 <template>
    <article>
        <div class="first-section">
        <main>
            <div class="section-one">
                
                <div class="so-text">
                    <div class="sub-text">
                        <p>PETER RODRIGUES BUTAO</p>
                    </div>
                    <div class="main-text">
                        <h1>UX / UI DESIGNER</h1>
                    </div>
                </div>
                <div class="so-icons">

                    <div class="soi-one">
                        <div class="soi-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="65" height="55" viewBox="0 0 65 55"><defs><clipPath id="a"><rect width="65" height="55" transform="translate(14 347)" fill="#fff" stroke="#707070" stroke-width="1"/></clipPath></defs><g transform="translate(-14 -347)" clip-path="url(#a)"><g transform="translate(19.078 347)"><g transform="translate(0)" fill="none" stroke="#fff" stroke-width="1.013"><ellipse cx="27.422" cy="27.5" rx="27.422" ry="27.5" stroke="none"/><ellipse cx="27.422" cy="27.5" rx="26.916" ry="26.994" fill="none"/></g><g transform="translate(21.938 21.771)"><path d="M0,9.625H10.969V11H0ZM0,4.812H10.969V8.25H0ZM4.8,0h6.17V3.437H4.8ZM0,0H3.428V3.437H0Z" fill="#fff" fill-rule="evenodd"/></g></g></g>
                            </svg>
                        </div>
                        <div class="soi-text">
                            <p>Interface Design</p>
                        </div>
                    </div>
                    <div class="soi-one">
                        <div class="soi-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="65" height="55" viewBox="0 0 65 55"><defs><clipPath id="a"><rect width="65" height="55" transform="translate(14 347)" fill="#fff" stroke="#707070" stroke-width="1"/></clipPath></defs><g transform="translate(-14 -347)" clip-path="url(#a)"><g transform="translate(19.078 347)"><g transform="translate(0)" fill="none" stroke="#fff" stroke-width="1.013"><ellipse cx="27.422" cy="27.5" rx="27.422" ry="27.5" stroke="none"/><ellipse cx="27.422" cy="27.5" rx="26.916" ry="26.994" fill="none"/></g><g transform="translate(21.938 21.771)"><path d="M0,9.625H10.969V11H0ZM0,4.812H10.969V8.25H0ZM4.8,0h6.17V3.437H4.8ZM0,0H3.428V3.437H0Z" fill="#fff" fill-rule="evenodd"/></g></g></g>
                            </svg>
                        </div>
                        <div class="soi-text">
                            <p>Development</p>
                        </div>
                    </div>
                    <div class="soi-one">
                        <div class="soi-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="65" height="55" viewBox="0 0 65 55"><defs><clipPath id="a"><rect width="65" height="55" transform="translate(14 347)" fill="#fff" stroke="#707070" stroke-width="1"/></clipPath></defs><g transform="translate(-14 -347)" clip-path="url(#a)"><g transform="translate(19.078 347)"><g transform="translate(0)" fill="none" stroke="#fff" stroke-width="1.013"><ellipse cx="27.422" cy="27.5" rx="27.422" ry="27.5" stroke="none"/><ellipse cx="27.422" cy="27.5" rx="26.916" ry="26.994" fill="none"/></g><g transform="translate(21.938 21.771)"><path d="M0,9.625H10.969V11H0ZM0,4.812H10.969V8.25H0ZM4.8,0h6.17V3.437H4.8ZM0,0H3.428V3.437H0Z" fill="#fff" fill-rule="evenodd"/></g></g></g>
                            </svg>
                        </div>
                        <div class="soi-text">
                            <p>Experience Design</p>
                        </div>
                    </div>


                </div>
            </div>
        </main>

        <footer>
            <div class="section-two">

                <g-link class="gts-sect">
                    <p>Get Started</p>
                    <p>🚀</p>
                </g-link>

                <div class="link-sect">
                            <ul class="bar">     
           
                                <li>
                                    <g-link>
                                            <g-image alt="facebook link" src="/facebook.svg" width="60" />
                                    </g-link>
                                </li>
                                <li>
                                    <g-link>
                                            <g-image alt="instagram link" src="/instagram.svg" width="60" />
                                    </g-link>
                                </li>
                                <li>
                                    <g-link>
                                            <g-image alt="twitter link" src="/twitter.svg" width="60" />
                                    </g-link>
                                </li>
                            </ul>
                </div>

            </div>
        </footer>
        </div>
    </article>
</template>

<style scoped>
ul{
    padding: 0;
    margin: 0;
}
li{
    margin: 0 auto;
    padding: 5px 10px;
}
.link-sect{
    position: fixed;
   margin-bottom: 60px;


}
.bar{
    display: block;
    background: #928787;
}
article{
    max-width: var(--mw);
    margin:0 auto;
    background: var(--pm);
   

}
.first-section{
    height: 100vh;
    margin: auto 0px;
    display: flex;
    flex-direction: column;
}
main{
    padding: 0 10px;
    flex:1;
    background-image: url("/bg.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-color: rgba(0, 0, 0, 0.426);
    background-blend-mode: multiply;
    transform: skewY(11deg);

}
.section-one{
    padding-top: 20vh;
    transform: skewY(-11deg);
}
main > .section-one > .so-text{
    border-left: 2px solid white;
    padding: 0px 10px;
}
.sub-text{
    color: var(--wc);
}
.main-text > h1{
    color: var(--pc);
    font-weight: 900;
    font-size: 2rem;
    line-height: 1;
}

.so-icons{
    display: flex;
    flex:1;
    justify-content: space-between;
    align-items: center;
    padding:10px 0px;

}
.soi-one{
    display: flex;
    flex-direction: column;
    align-items: center;
}
.soi-text{
    color: var(--wc);
    font-size: 0.9rem
}
footer{
    position: relative;
    margin-bottom: 10px;
    padding-top: 8vh;
}
footer > .section-two {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.gts-sect{
    margin-top: auto;
    margin-left: auto;
    margin-right: 3px;
    display: flex;
    border: var(--wc) solid 1px;
    padding:5px 10px;
    
}
.gts-sect > p{
    padding: 0;
    margin: 0;
    padding: 0px 5px;
    color: var(--wc);
}
</style>