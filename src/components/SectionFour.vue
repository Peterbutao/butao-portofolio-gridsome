<template>
    <article>
        <div class="frth-section">
            <header>
                <div class="title">
                    <h1>SERVICES</h1>
                </div>
            </header>
            <main>
                <div class="cards">

                    <div class="card">
                        <div class="cd">

                            <div class="section-one">
                                <g-image
                                src="/services1.svg"
                                alt="services icons"
                                />
                            </div>
                            <div class="section-two">
                                <h1>APP DEVELOPMENT</h1>
                            </div>

                        </div>
                    </div>

                    <div class="card">
                        <div class="cd">

                            <div class="section-one">
                                <g-image
                                src="/services2.svg"
                                alt="services icons"
                                />
                            </div>
                            <div class="section-two">
                                <h1>UX DESIGN</h1>
                            </div>

                        </div>
                    </div>

                    <div class="card">
                        <div class="cd">

                            <div class="section-one">
                                <g-image
                                src="/services3.svg"
                                alt="services icons"
                                />
                            </div>
                            <div class="section-two">
                                <h1>WEB DEVELOPMENT</h1>
                            </div>

                        </div>
                    </div>

                    <div class="card">
                        <div class="cd">

                            <div class="section-one">
                                <g-image
                                src="/services4.svg"
                                alt="services icons"
                                />
                            </div>
                            <div class="section-two">
                                <h1>SITE MANAGEMENT</h1>
                            </div>

                        </div>
                    </div>


                </div>
            </main>
        </div>
    </article>
</template>
<style scoped>
article{
    padding: 0 10px;
    background: var(--pm);
    max-width: var(--mw);
    margin: 0 auto;
}
.title > h1{
    color: var(--pc);
    padding: 10px 0;
}
.card{
    padding: 15px 10px;
}
.cd{
    padding: 15px 0;
    background: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
</style>