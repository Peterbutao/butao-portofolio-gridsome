<template>
    <article>
        <div class="snd-section">
            <header>
                <div class="title">
                    <h1>PROJECTS</h1>
                </div>
            </header>
            <main>
                <div class="cards" v-bind:key="project.name" v-for="project in projects">
                    
                    <div class="card">
                        <div class="cd">

                            <div class="section-one">
                                <g-image
                                    class="pi"
                                    alt="project icon" 
                                    width="70px"
                                    :src="`${project.logo}.png`" />                       
                            </div>
                            <div class="section-two">
                                <div class="head-text">
                                    <h1>{{project.name}}</h1>
                                </div>
                                <div class="para-text">
                                    <p>
                                        {{project.meta}}
                                    </p>
                                    <div class="more">
                                        <a href="/">VISIT</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>


                </div>
            </main>
            <footer>
                <a  href="https://*" target="_blank" class="foot-link">
                    <div class="ftl-text">
                        <p>GITHUB REPOS</p>
                    </div>
                    <div class="ftl-icons">
                        <g-image class="git" src="/github.svg" width="35px" alt="github" />
                    </div>
                </a>
            </footer>
        </div>
    </article>
</template>
<script>
export default {
    name: "SectionTwo",
    props: ["projects"]
}
</script>
<style scoped>
.git{
    border-left: solid 2px white;
    padding-left: 10px;
}
footer{
    padding: 10px;
}
.foot-link{
    background:#ffffff50;
    padding: 5px 10px;
    font-weight: 700;
    display: flex;
    align-items: center;
    color: var(--tc);
    justify-content: space-between;
    
}

article{
    padding: 0 10px;
    max-width: var(--mw);
    margin: auto;
    background: var(--pm);

}
.title > h1{
    color: var(--pc);
    font-weight: 800;
    font-size: 1.5rem;
    margin: 0;
    padding: 10px 0;

}
.more{
    padding: 10px 0;
}
.pi{
    width: 45px;
    padding: 8px;
    border-right: 1px solid var(--pm);
}
.head-text > h1{
    margin: 0;
    padding: 5px 0px;
    color: var(--tc);
    font-size: 0.9rem;
    font-weight: 650;
    opacity: 80%;
}
.para-text{
    line-height: 1.2;
    font-size: 0.9rem;
    font-weight: 600;
    opacity: 70%;

}
.card{
    padding: 15px 10px;
}
.cd{
    background: white;
    display: flex;
    align-items: center;
    padding: 2px;
    border-radius: 5px;

}
.section-two{
    padding:0;
    margin:0;
    padding-left: 10px;
}

</style>