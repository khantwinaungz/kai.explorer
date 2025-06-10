// Mobile Menu Toggle
document.querySelector('.mobile-menu').addEventListener('click', function() {
    const nav = document.querySelector('nav');
    nav.style.display = nav.style.display === 'flex' ? 'none' : 'flex';
    
    // Adjust for mobile view
    if (window.innerWidth <= 768) {
        if (nav.style.display === 'flex') {
            nav.style.flexDirection = 'column';
            nav.style.position = 'absolute';
            nav.style.top = '100%';
            nav.style.left = '0';
            nav.style.width = '100%';
            nav.style.backgroundColor = 'white';
            nav.style.padding = '20px 0';
            nav.style.boxShadow = '0 5px 10px rgba(0,0,0,0.1)';
            
            const navItems = nav.querySelectorAll('li');
            navItems.forEach(item => {
                item.style.margin = '10px 0';
                item.style.textAlign = 'center';
            });
        }
    }
});

// Close menu when clicking outside
document.addEventListener('click', function(e) {
    const nav = document.querySelector('nav');
    const mobileMenu = document.querySelector('.mobile-menu');
    
    if (window.innerWidth <= 768 && nav.style.display === 'flex') {
        if (!nav.contains(e.target) && !mobileMenu.contains(e.target)) {
            nav.style.display = 'none';
        }
    }
});

// Newsletter form submission
document.querySelector('.newsletter form')?.addEventListener('submit', function(e) {
    e.preventDefault();
    const email = this.querySelector('input').value;
    if (email && validateEmail(email)) {
        alert('Thank you for subscribing!');
        this.reset();
    } else {
        alert('Please enter a valid email address');
    }
});

function validateEmail(email) {
    const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return re.test(email);
}

// Smooth scrolling for anchor links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            window.scrollTo({
                top: target.offsetTop - 80,
                behavior: 'smooth'
            });
        }
    });
});
