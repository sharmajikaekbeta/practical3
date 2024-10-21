# practical3
body, html {
    margin: 0;
    padding: 0;
    height: 100%;
}


.image-container {
    width: 100%;
    height: 100vh;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
}


.responsive-image {
    width: 1250px; /* Double the image width to allow full sliding */
    height: 1250px; /* Double the image height to allow full sliding */
    position: relative;
    transition: transform 0.3s ease-in-out;
}


@media screen and (max-width: 1600px) {
    .responsive-image {
        transform: translateX(-625px); /* Show top-right */
    }
}


@media screen and (max-width: 1400px) {
    .responsive-image {
        transform: translateY(-625px); /* Show bottom-left */
    }
}


@media screen and (max-width: 1200px) {
    .responsive-image {
        transform: translate(-625px, -625px); /* Show bottom-right */
    }
}


@media screen and (max-width: 1000px) {
    .responsive-image {
        transform: translateY(-625px); /* Show bottom-left again */
    }
}


@media screen and (max-width: 800px) {
    .responsive-image {
        transform: translateX(-625px); /* Show top-right again */
    }
}


@media screen and (max-width: 600px) {
    .responsive-image {
        transform: translateX(0px); /* Show top-left */
    }
}































body, html {
    margin: 0;
    padding: 0;
    height: 100%;
}


.image-container {
    width: 100%;
    height: 100vh;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
}


.responsive-image {
    width: 2000px; /* Assuming each image is 400px wide and there are 5 columns */
    height: 1200px; /* Assuming each image is 600px tall and there are 2 rows */
    position: relative;
    transition: transform 0.3s ease-in-out;
}


/* Media queries to show different parts of the image */


@media screen and (min-width: 1201px) {
    .responsive-image {
        transform: translate(0, 0); /* Show top-left ("How the customer explained it") */
    }
}


@media screen and (max-width: 1200px) and (min-width: 1101px) {
    .responsive-image {
        transform: translateX(-400px); /* Show second image on the top row ("How the Project Leader understood it") */
    }
}


@media screen and (max-width: 1100px) and (min-width: 1001px) {
    .responsive-image {
        transform: translateX(-800px); /* Show third image on the top row ("How the Analyst designed it") */
    }
}


@media screen and (max-width: 1000px) and (min-width: 901px) {
    .responsive-image {
        transform: translateX(-1200px); /* Show fourth image on the top row */
    }
}


@media screen and (max-width: 900px) and (min-width: 801px) {
    .responsive-image {
        transform: translateX(-1600px); /* Show fifth image on the top row */
    }
}


@media screen and (max-width: 800px) and (min-width: 701px) {
    .responsive-image {
        transform: translateY(-600px); /* Show first image on the second row ("How the project was documented") */
    }
}


@media screen and (max-width: 700px) and (min-width: 601px) {
    .responsive-image {
        transform: translate(-400px, -600px); /* Show second image on the second row */
    }
}


@media screen and (max-width: 600px) and (min-width: 501px) {
    .responsive-image {
        transform: translate(-800px, -600px); /* Show third image on the second row */
    }
}


@media screen and (max-width: 500px) and (min-width: 401px) {
    .responsive-image {
        transform: translate(-1200px, -600px); /* Show fourth image on the second row */
    }
}


@media screen and (max-width: 400px) {
    .responsive-image {
        transform: translate(-1600px, -600px); /* Show last image ("What the customer really needed") */
    }
}



