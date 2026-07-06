# karnataka-tourism-1<!-- ADD THIS CODE BEFORE </body> TAG -->

<!-- ================= BOOKING FORM ================= -->

<section class="booking-section" id="booking">

    <h2 class="section-title">Book Your Vehicle</h2>

    <form class="booking-form">

        <input type="text" placeholder="Your Full Name" required>

        <input type="tel" placeholder="Mobile Number" required>

        <input type="text" placeholder="Pickup Location" required>

        <input type="text" placeholder="Drop Location" required>

        <input type="date" required>

        <select required>
            <option value="">Select Vehicle</option>
            <option>Sedan</option>
            <option>Innova</option>
            <option>Tempo Traveller</option>
            <option>Mini Bus</option>
            <option>Luxury Bus</option>
        </select>

        <textarea placeholder="Message"></textarea>

        <button type="submit">Book Now</button>

    </form>

</section>

<!-- ================= CUSTOMER REVIEWS ================= -->

<section class="reviews">

    <h2 class="section-title">Customer Reviews</h2>

    <div class="review-container">

        <div class="review-box">
            ⭐⭐⭐⭐⭐
            <p>
                Excellent service and very professional driver.
                Highly recommended for family trips.
            </p>
            <h4>- Ramesh</h4>
        </div>

        <div class="review-box">
            ⭐⭐⭐⭐⭐
            <p>
                Tempo Traveller was clean and comfortable.
                Affordable pricing.
            </p>
            <h4>- Priya</h4>
        </div>

        <div class="review-box">
            ⭐⭐⭐⭐⭐
            <p>
                Best tours and travels service in Bangalore.
                On-time pickup and safe driving.
            </p>
            <h4>- Naveen</h4>
        </div>

    </div>

</section>

<!-- ================= GALLERY ================= -->

<section class="gallery">

    <h2 class="section-title">Travel Gallery</h2>

    <div class="gallery-grid">

        <img src="https://images.unsplash.com/photo-1503376780353-7e6692767b70?q=80&w=1200&auto=format&fit=crop">

        <img src="https://images.unsplash.com/photo-1519641471654-76ce0107ad1b?q=80&w=1200&auto=format&fit=crop">

        <img src="https://images.unsplash.com/photo-1544620347-c4fd4a3d5957?q=80&w=1200&auto=format&fit=crop">

        <img src="https://images.unsplash.com/photo-1570129477492-45c003edd2be?q=80&w=1200&auto=format&fit=crop">

    </div>

</section>

<!-- ================= GOOGLE MAP ================= -->

<section class="map-section">

    <h2 class="section-title">Our Location</h2>

    <iframe
    src="https://maps.google.com/maps?q=Ramamurthy%20Nagar%20Bangalore&t=&z=13&ie=UTF8&iwloc=&output=embed"
    width="100%"
    height="400"
    style="border:0;"
    allowfullscreen=""
    loading="lazy">
    </iframe>

</section>

<!-- ================= ONLINE PAYMENT ================= -->

<section class="payment-section">

    <h2 class="section-title">Online Payment</h2>

    <p style="text-align:center;">
        Make secure online payments using UPI, Google Pay, PhonePe or Paytm.
    </p>

    <div style="text-align:center;margin-top:20px;">
        <a href="https://pay.google.com/" class="btn">
            Pay Now
        </a>
    </div>

</section>

<!-- ================= VIDEO BACKGROUND ================= -->

<style>

/* VIDEO HERO */

.video-hero{
    position:relative;
    width:100%;
    height:100vh;
    overflow:hidden;
}

.video-hero video{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    object-fit:cover;
}

.video-overlay{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:rgba(0,0,0,0.6);
    display:flex;
    justify-content:center;
    align-items:center;
    flex-direction:column;
    color:#fff;
    text-align:center;
}

/* BOOKING FORM */

.booking-section{
    background:#f5f5f5;
    padding:70px 5%;
}

.booking-form{
    max-width:800px;
    margin:auto;
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:20px;
}

.booking-form input,
.booking-form select,
.booking-form textarea{
    padding:15px;
    border:1px solid #ccc;
    border-radius:5px;
    width:100%;
}

.booking-form textarea{
    grid-column:span 2;
    height:120px;
}

.booking-form button{
    grid-column:span 2;
    padding:15px;
    background:#0056b3;
    color:#fff;
    border:none;
    font-size:18px;
    border-radius:5px;
    cursor:pointer;
}

/* REVIEWS */

.review-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.review-box{
    background:#fff;
    padding:25px;
    border-radius:10px;
    box-shadow:0 4px 12px rgba(0,0,0,0.1);
    text-align:center;
}

/* GALLERY */

.gallery{
    background:#f9f9f9;
}

.gallery-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.gallery-grid img{
    width:100%;
    height:250px;
    object-fit:cover;
    border-radius:10px;
    transition:0.3s;
}

.gallery-grid img:hover{
    transform:scale(1.05);
}

/* ANIMATIONS */

.service-box,
.fleet-card,
.review-box,
.gallery-grid img{
    animation:fadeInUp 1s ease;
}

@keyframes fadeInUp{

    from{
        opacity:0;
        transform:translateY(40px);
    }

    to{
        opacity:1;
        transform:translateY(0);
    }

}

/* DARK LUXURY DESIGN */

body{
    background:#111;
    color:#eee;
}

section{
    background:#111;
}

.service-box,
.review-box,
.fleet-card{
    background:#1c1c1c;
    color:#fff;
}

.section-title{
    color:#ffcc00;
}

/* MOBILE */

@media(max-width:768px){

    .booking-form{
        grid-template-columns:1fr;
    }

    .booking-form textarea,
    .booking-form button{
        grid-column:span 1;
    }

}

</style>

<!-- ================= SIMPLE BOOKING ALERT ================= -->

<script>

document.querySelector(".booking-form")
.addEventListener("submit", function(e){

    e.preventDefault();

    alert("Thank You! Your booking request has been submitted.");

});

</script>
