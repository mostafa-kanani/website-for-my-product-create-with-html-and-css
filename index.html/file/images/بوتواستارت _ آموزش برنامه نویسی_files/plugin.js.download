(function($) {
    "use strict";

    $(window).on("load", function() {

        // Download
        if ($('.download_items').length) {
            $('.download-filter ul li').on("click", function() {
                $(".download-filter ul li").removeClass("select-cat");
                $(this).addClass("select-cat");
            });
        }

        // Newest
        if ($('.newest_items').length) {
            $('.newest-filter ul li').on("click", function() {
                $(".newest-filter ul li").removeClass("select-cat");
                $(this).addClass("select-cat");
            });
        }


    }); // window load end 3

    // AJAX Search
    $(document).mouseup(function(e) {

        var searchresuls = $(".sidebar-search");

        // if the target of the click isn't the container nor a descendant of the container
        if (!searchresuls.is(e.target) && searchresuls.has(e.target).length === 0) {
            $("#datafetch").hide();
        }
    });

    // Products Tooltip
    $(".sit-preview").smartImageTooltip({ previewTemplate: "envato", imageWidth: "500px" });

    // Masonry
    $('.masonry-grid').masonry({
        itemSelector: '.masonry-grid>div'
    });

    // Banner Carousel
    $(window).on("load", function() {
        $('.banner').show();
    });

    // Slick RTL Support
    function rtl_slick() {
        if ($('body').hasClass("rtl")) {
            return true;
        } else {
            return false;
        }
    }

    // Elementor front-end
    $(window).on('elementor/frontend/init', function() {

        elementorFrontend.hooks.addAction('frontend/element_ready/testimonials.default', function($scope, $) {

          var carousel = $('.testimonials-wrapper .owl-carousel');

              if ( carousel.length ) {

                carousel.each( function () {

                    var owl = $(this),
                        autoplay = owl.data('autoplay'),
                        pagination = owl.data('pagination') ? owl.data('pagination') : false,
                        loop = owl.data('loop'),
                        slide_items = owl.data('slider-items');

                    owl.owlCarousel({
                      items: slide_items,
                      responsive: {
                          979: {
                              items: slide_items
                          },
                          768: {
                              items: 2
                          },
                          479: {
                              items: 1
                          },
                          0: {
                              items: 1
                          }
                      },
                        dots: pagination,
                        nav: true,
                        rtl: true,
                        autoheight: true,
                        autoplay: autoplay,
                        navText: ['<i class="fa fa-angle-left"></i>','<i class="fa fa-angle-right"></i>'],
                        loop: loop,
                    });

                });
              }

        });


		elementorFrontend.hooks.addAction('frontend/element_ready/Carousel_Products.default', function($scope, $) {

            var carousel = $('.courses-holder .owl-carousel');

                if ( carousel.length ) {

                    carousel.each( function() {
                      var owl = $(this),
                      autoplay = owl.data('autoplay'),
                      pagination = owl.data('pagination') ? owl.data('pagination') : false,
                      navigation = owl.data('navigation') ? owl.data('navigation') : false,
                      loop = owl.data('loop'),
                      slide_items = owl.data('slider-items');

                  owl.owlCarousel({
                      items: slide_items,
                      responsive: {
                          979: {
                              items: slide_items
                          },
                          768: {
                              items: 2
                          },
                          479: {
                              items: 1
                          },
                          0: {
                              items: 1
                          }
                      },
                      dots: pagination,
                      nav: navigation,
                      autoplay: autoplay,
                      autoheight: true,
                      navText: ['<i class="fa fa-angle-left"></i>','<i class="fa fa-angle-right"></i>'],
                      rtl: true,
                      loop: loop,

                            onRefreshed: function() {
                                $(window).resize();
                            }
                        });
                    });

                }

        });


		elementorFrontend.hooks.addAction('frontend/element_ready/blog-carousel.default', function($scope, $) {

            var carousel = $('.blog-posts-holder .owl-carousel');

                if ( carousel.length ) {

                    carousel.each( function() {
                      var owl = $(this),
                      autoplay = owl.data('autoplay'),
                      pagination = owl.data('pagination') ? owl.data('pagination') : false,
                      navigation = owl.data('navigation') ? owl.data('navigation') : false,
                      loop = owl.data('loop'),
                      slide_items = owl.data('slider-items');

                  owl.owlCarousel({
                      items: slide_items,
                      responsive: {
                          979: {
                              items: slide_items
                          },
                          768: {
                              items: 2
                          },
                          479: {
                              items: 1
                          },
                          0: {
                              items: 1
                          }
                      },
                      dots: pagination,
                      nav: navigation,
                      autoplay: autoplay,
                      autoheight: true,
                      navText: ['<i class="fa fa-angle-left"></i>','<i class="fa fa-angle-right"></i>'],
                      rtl: true,
                      loop: loop,

                            onRefreshed: function() {
                                $(window).resize();
                            }
                        });
                    });

                }

        });


        elementorFrontend.hooks.addAction('frontend/element_ready/Swiper_Products.default', function($scope, $) {

          let swiper = new Swiper ('.swiper-container-5', {
            effect: 'coverflow',
            centeredSlides: true,
            slidesPerView: "auto",
            grabCursor: true,
            initialSlide: 2,
            speed: 700,
            keyboardControl: true,
            coverflowEffect: {
              rotate: 0,
              stretch: 50,
              depth: 400,
              modifier: 1,
              slideShadows: true,
            },
            pagination: {
              el: '.swiper-pagination',
              clickable: true,
            },
            navigation: {
              nextEl: '.swiper-button-next',
              prevEl: '.swiper-button-prev',
            },
          });

            });



            elementorFrontend.hooks.addAction('frontend/element_ready/blog-podcast.default', function($scope, $) {

              let swiper = new Swiper('.blog-slider', {
								spaceBetween: 30,
								effect: 'fade',
								loop: true,
								grabCursor: true,
								// autoHeight: true,
								pagination: {
								el: '.blog-slider__pagination',
								clickable: true,
								}
							});

                });


    });


})(jQuery);
