document.addEventListener("DOMContentLoaded", function() {
    const links = document.querySelectorAll("nav ul li a");
    const backToTopButton = document.getElementById("back-to-top");

    if (!links.length) {
        console.error("No navigation links found");
        return;
    }
    if (!backToTopButton) {
        console.error("Back-to-top button not found");
        return;
    }

    links.forEach(link => {
        link.addEventListener("click", function(event) {
            event.preventDefault();
            const targetId = link.getAttribute("href").substring(1);
            const targetElement = document.getElementById(targetId);

            if (!targetElement) {
                console.error(`Target element with id ${targetId} not found`);
                return;
            }

            window.scrollTo({
                top: targetElement.offsetTop,
                behavior: "smooth"
            });
        });
    });
    window.addEventListener("scroll", function() {
        if (window.scrollY > 200) {
            backToTopButton.style.display = "block";
        } else {
            backToTopButton.style.display = "none";
        }
    });

    backToTopButton.addEventListener("click", function() {
        window.scrollTo({
            top: 0,
            behavior: "smooth"
        });
    });
});
