<template>
    <div id="Home">
        <div class="home-container">
            <section class="top-container">
                <header class="showcase">
                    <h1>Twice Jihyo</h1>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Ipsam, porro? Eius praesentium corrupti ut tempore.
                    </p>
                    <a href="#" class="btn">Read More</a>
                </header>
                <div class="top-box top-box-a">
                    <h4>Membership</h4>
                    <p class="price">$199/mo</p>
                    <a href="#" class="btn">Buy Now</a>
                </div>
                <div class="top-box top-box-b">
                    <h4>Pro Membership</h4>
                    <p class="price">$299/mo</p>
                    <a href="#" class="btn">Buy Now</a>
                </div>
            </section>

            <section class="boxes">
                <div class="box">
                    <i class="fas fa-chart-pie fa-4x"></i>
                    <h3>Analytics</h3>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Hic, repellat?
                    </p>
                </div>
                <div class="box">
                    <i class="fas fa-globe fa-4x"></i>
                    <h3>Marketing</h3>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Hic, repellat?
                    </p>
                </div>
                <div class="box">
                    <i class="fas fa-cog fa-4x"></i>
                    <h3>Development</h3>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Hic, repellat?
                    </p>
                </div>
                <div class="box">
                    <i class="fas fa-users fa-4x"></i>
                    <h3>Support</h3>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Hic, repellat?
                    </p>
                </div>
            </section>

            <section class="info">
                <img
                    src="https://scontent-yyz1-1.xx.fbcdn.net/v/t1.6435-9/p370x247/83827361_106565387559634_8760722690920153088_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=85a577&_nc_ohc=BfxjE7m5di8AX9pW6eq&_nc_ht=scontent-yyz1-1.xx&oh=00_AT_4S0RFcWdLErwTQCxyyKp-xtGbeMgD3X2Eq9DBUtjIjQ&oe=61E1DBF4"
                    alt=""
                />
                <div>
                    <h2>Your Business On The Web</h2>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Autem quos maiores necessitatibus beatae incidunt
                        accusantium, molestias adipisci, magnam tempora
                        accusamus, veniam ea. Fuga laborum corrupti voluptatem
                        sit unde, expedita dolore!
                    </p>
                    <a href="#" class="btn">Learn More</a>
                </div>
            </section>

            <section class="portfolio">
                <img src="https://source.unsplash.com/random/200x200" alt="" />
                <img src="https://source.unsplash.com/random/201x200" alt="" />
                <img src="https://source.unsplash.com/random/202x200" alt="" />
                <img src="https://source.unsplash.com/random/203x200" alt="" />
                <img src="https://source.unsplash.com/random/204x200" alt="" />
                <img src="https://source.unsplash.com/random/205x200" alt="" />
                <img src="https://source.unsplash.com/random/206x200" alt="" />
                <img src="https://source.unsplash.com/random/207x200" alt="" />
                <img src="https://source.unsplash.com/random/208x200" alt="" />
                <img src="https://source.unsplash.com/random/209x200" alt="" />
            </section>

            <footer>
                <p>Harrison Kim &copy; 2021</p>
            </footer>
        </div>
    </div>
</template>

<script>
export default {
    name: "Home",
};
</script>

<style scoped>
#Home {
    color: var(--dark);
    padding: 30px 50px;
    line-height: 1.4;
}

.home-container {
    display: grid;
    grid-gap: 20px;
}

.btn {
    background: var(--dark);
    color: var(--light);
    padding: 0.6rem 1.3rem;
    text-decoration: none;
    border: 0;
    display: inline-block;
}

img {
    max-width: 100%;
}

/* Top Container */
.top-container {
    display: grid;
    grid-gap: 20px;
    grid-template-areas:
        "showcase showcase top-box-a"
        "showcase showcase top-box-b";
}

.showcase {
    grid-area: showcase;
    min-height: 400px;
    background: url("https://i.pinimg.com/originals/59/30/0e/59300ee357d34a144d518920d8a574ea.jpg");
    background-size: cover;
    background-position: center;
    padding: 3rem;
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: center;
    box-shadow: var(--shadow);
}

.showcase h1 {
    font-size: 4rem;
    margin-bottom: 0;
    color: var(--light);
}

.showcase p {
    font-size: 1.3rem;
    margin-top: 0;
    color: var(--light);
}

/* Top Box */
.top-box {
    background: var(--primary);
    display: grid;
    align-items: center;
    justify-items: center;
    box-shadow: var(--shadow);
    padding: 1.5rem;
}

.top-box .price {
    font-size: 2.5rem;
}

.top-box-a {
    grid-area: top-box-a;
}

.top-box-b {
    grid-area: top-box-b;
}

/* Boxes */
.boxes {
    display: grid;
    grid-gap: 20px;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
}

.box {
    background: var(--primary);
    text-align: center;
    padding: 1.5rem 2rem;
    box-shadow: var(--shadow);
}

/* Info */
.info {
    background: var(--primary);
    box-shadow: var(--shadow);
    display: grid;
    grid-gap: 30px;
    grid-template-columns: repeat(2, 1fr);
    padding: 3rem;
}

/* Portfolio */
.portfolio {
    display: grid;
    grid-gap: 20px;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
}

.portfolio img {
    width: 100%;
    box-shadow: var(--shadow);
}

footer {
    margin-top: 2rem;
    background: var(--dark);
    color: var(--light);
    text-align: center;
    padding: 1rem;
}

/* Media Queries */
@media (max-width: 700px) {
    .top-container {
        grid-template-areas:
            "showcase showcase"
            "top-box-a top-box-b";
    }

    .showcase h1 {
        font-size: 2.5rem;
    }

    .info {
        grid-template-columns: 1fr;
    }

    .info div p {
        margin: 1.3rem 0;
    }

    .info .btn {
        display: block;
        text-align: center;
        margin: auto;
    }
}

@media (max-width: 500px) {
    .top-container {
        grid-template-areas:
            "showcase"
            "top-box-a"
            "top-box-b";
    }
}
</style>
