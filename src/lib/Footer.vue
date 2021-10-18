<template>

<article>
    <div class="footer">
        <div class="section-one">
            <ul>
                <li>
                    <h1>CONNECT</h1>
                </li>
                <li>
                    <a href="/">Linkedin</a>
                </li>
                <li>
                    <a href="/">Github</a>
                </li>
                <li>
                    <a href="/">Dribble</a>
                </li>
                <li>
                    <a href="/">Behance</a>
                </li>
            </ul>
            
            <ul>
                <li>
                    <h1>FEEDBACK</h1>
                    <input type="text" name="text" placeholder="enter feedback" id="txt">
                </li>

            </ul>
        </div>
        <div class="section-two">
            <div class="copy">
                <p>copyright © peterbutao 2021</p>
            </div>
            <hr>
            <div class="brand">
                <h1>BUTAO UX/UI DEV</h1>
            </div>
            <br>
            <div class="arck">
                <span>created with</span>
                <span class="grid">
                    <g-image src="~/favicon.png" width="25px" />
                </span>
                <span>by </span>
                <span style="color:var(--pm)"> BUTAO</span>
            </div>
        </div>
    </div>
</article>
</template>

<script>
export default {
    name: "Footer"
}
</script>
<style scoped>
article{
    padding: 0 10px;
    margin: 0 auto;
    max-width: var(--mw);
}
input{
    border: none;
    background: var(--pm);
    opacity: 50%;
    border-radius: 3rem;
    padding: 10px;
    color: var(--wc);

}
input:focus{
    outline: none;

}
input::placeholder{
    color: white;
}
ul{
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;

}
li{
    padding:10px 0;
}
.grid{
    padding: 0 5px;
}
.section-two{
    padding: 8vh 0;
    text-align: center;
}
</style>