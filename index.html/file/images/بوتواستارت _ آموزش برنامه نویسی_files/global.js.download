(function($) {
    'use strict';

    jQuery(document).ready(function($) {

        $(document).on('click', '.course-section-title-elementory.cursor-pointer', function(event) {
            event.preventDefault();
            $(this).parent().toggleClass('active');
            $(this).next('.panel-group').slideToggle(300);
        });

        $(document).on('click', '.notif-row', function(event) {
            event.preventDefault();
            $(this).parent().toggleClass('active');
            $(this).next('.notif-content').slideToggle(300);
        });

    });
})(jQuery);

jQuery(function($) {
			$(".meter > span").each(function() {
				$(this)
					.data("origWidth", $(this).width())
					.width(0)
					.animate({
						width: $(this).data("origWidth")
					}, 1200);
			});
		});

jQuery(function($) {
	var upperLimit = 100;
	var scrollElem = $('a#scroll-to-top');
	var scrollSpeed = 600;
	var scrollStyle = 'swing';
	scrollElem.hide();
	$(window).scroll(function () {
		var scrollTop = $(document).scrollTop();
		if ( scrollTop > upperLimit ) {
			$(scrollElem).stop().fadeTo(300, 1);
		}else{
			$(scrollElem).stop().fadeTo(300, 0);
		}
	});

	$(scrollElem).click(function(){
		$('html, body').animate({scrollTop:0}, scrollSpeed, scrollStyle ); return false;
	});

  $('.site-navigation a[href*="#"]:not([href="#"]):not([href^="#tab"])').click(function()
  {
    if (location.pathname.replace(/^\//,'') == this.pathname.replace(/^\//,'')
        || location.hostname == this.hostname)
    {

      var target = $(this.hash),
      headerHeight = $(".primary-header").height() + 5; // Get fixed header height

      target = target.length ? target : $('[name=' + this.hash.slice(1) +']');

      if (target.length)
      {
        $('html,body').animate({ scrollTop: target.offset().top }, scrollSpeed, scrollStyle );
        return false;
      }
    }
  });
});

function dumpit(t) {
    console.log(t)
}
jQuery.fn.outerHTML = function(t) {
        return t ? this.before(t).remove() : jQuery("<p>").append(this.eq(0).clone()).html()
    }, jQuery.extend({
        stripTags: function(t) {
            return t ? t.replace(/(<([^>]+)>)/gi, "") : ""
        }
    }),
    function(t) {

      t(function() {
            var e = t("#categories_navigation"),
                i = "click" == e.data("action") ? "click" : "mouseenter mouseleave",
                a = t("#categories_navigation_toggle");
            "click" == i && e.find("> ul > li:first-child").addClass("active"), a.on(i, function(a) {
                "click" == i && a.preventDefault(), t(this).toggleClass("opened"), e.toggleClass("opened")
            }), "click" == i && t(document).mouseup(function(t) {
                a.is(t.target) || e.is(t.target) || 0 !== e.has(t.target).length || !e.hasClass("opened") || (e.removeClass("opened"), a.removeClass("opened"))
            }), e.find(" > ul > li > a").on(i, function(a) {
                "click" == i && a.preventDefault();
                var n = t(this).parent(),
                    s = n.find(" > ul");
                t(" > ul > li > ul", e).css({
                    visibility: "hidden",
                    opacity: "0"
                }), s.css({
                    visibility: "visible",
                    opacity: "1"
                }), "click" == i && (t(" > ul > li", e).removeClass("active"), n.addClass("active"))
            })
        })
    }(jQuery);



(function($) {
    'use strict';

    jQuery(document).ready(function($) {

        $(document).on('click', 'ul.wcdlar_download_list li a.title', function(event) {
            event.preventDefault();
            $(this).parent().toggleClass('active');
            $(this).next('.sub_items').slideToggle(300);
        });

    });
})(jQuery);


(function($) {
    'use strict';

    jQuery(document).ready(function($) {

        $(document).on('click', 'h5.course-section-title.cursor-pointer', function(event) {
            event.preventDefault();
            $(this).parent().toggleClass('active');
            $(this).next('.panel-group').slideToggle(300);
        });

    });
})(jQuery);

var cdbTheme=cdbTheme||{};

;(function($, window, undefined) {

    "use strict";

    $(document).ready(function () {

        // Define global vars
        cdbTheme.$body          = $("body");
        cdbTheme.$window        = $(window);
        cdbTheme.$header        = $('.site-header');


        // Sticky Header
        function setupFixedHeader() {


            // Initialize sticky menu
            var $watcherElement = cdbTheme.$header.find('.site-header-inner');

            var watcher = window.scrollMonitor.create($watcherElement.get(0), {top: cdbTheme.$body.hasClass('admin-bar2') ? 0 : 0}),
                $spacer = null,
                headerHeight = cdbTheme.$header.outerHeight(),
                minWidth = 768;

            $spacer = cdbTheme.$header.prev();

            $spacer.height(headerHeight);

            watcher.lock();

            watcher.partiallyExitViewport(function() {

                if(minWidth > $(window).width()) {
                    return;
                }

                cdbTheme.$header.addClass('fixed-active');
                $spacer.removeClass('hidden');
            });

            watcher.fullyEnterViewport(function() {

                if(minWidth > $(window).width()) {
                    return;
                }

                cdbTheme.$header.removeClass('fixed-active');
                $spacer.addClass('hidden');


            });

        }

        if(cdbTheme.$header.hasClass('cdb-header-fixed')) {
            setupFixedHeader();
            cdbTheme.$body.addClass('fixed-body');
        }
				if(cdbTheme.$header.hasClass('cdb-header-fixed-2')) {
            setupFixedHeader();
            cdbTheme.$body.addClass('fixed-body-2');
        }
    });
} )(jQuery, window);

var studiareTheme;

(function($) {
    'use strict';

    studiareTheme = (function() {

        var body = $('body');

        return {

            init: function() {
                this.studiare_preloader();
								this.off_canvas_side_cart();
                this.header_search();
                this.dropdwon_arrow();
								this.dropdwon_arrow_mobile();
								this.dropdwon_arrow_sidebar();
                this.back_to_top();
                this.off_canvas_navigation();
								this.off_canvas_my_account_navigation();
								this.study_mode();
                this.modal_login_form();
								this.modal_advice_form();
                this.select_to_select2();
                this.courses_layout_switch();
                this.header_mini_cart();
								this.dropdown_menu();
                this.sticky_sidebar();
//                 this.video_popup();
                this.portfolioFilter();
                this.animatedCounter();
                this.courseCategories();
                this.blogMasonry();
                this.testimonialsCarousel();
                this.coursePanel();
                this.countDownTimer();
                this.galleryLightbox();
                this.galleryCarousel();
                this.coursesCarousel();
                this.blogpostsCarousel();
                this.megamenupostion();
								this.log_reg();
								this.box_download();
            },

            /**
             * Preloader Page
             */
            studiare_preloader: function() {
                var $preload = $('.studiare-preloader');
                var is_user = false;
                if ($('body').hasClass('logged-in')) {
                    is_user = true;
                }

                if (is_user || (top === self)) {
                    // if logined and not in a iframe.
                    if ($preload.length > 0) {
                        $preload.fadeOut(600, function () {
                            $preload.remove();
                        });
                    }
                }
            },


						/**
			 * Off Canvas Side Cart
			 */
			off_canvas_side_cart: function() {

					$('.header-cart-icon').on('click', function(ev) {
							ev.preventDefault();

							body.toggleClass('side-off-canvas-open');
					});

					$('.off-canvas-overlay').on('click', function(ev) {
							ev.preventDefault();

							body.removeClass('side-off-canvas-open');
					});

			},

            /**
             * Header Search
             */
            header_search: function() {
                var searchInput = $('.site-header .search-input'),
                    searchOpener = $('.top-bar-search .search-form-opener'),
                    searchOpenerIcon = searchOpener.find('i');

                $(document).on("click", ".search-form-opener, .search-capture-click", function (ev) {
                    ev.preventDefault();

                    if ( body.hasClass('search-active') ) {

                        body.removeClass('search-active');


                    } else {

                        body.addClass('search-active');
                        setTimeout(function(){searchInput.focus();}, 700);
                    }

                });

								$(window).scroll(function() {
		    var scroll = $(window).scrollTop();

		     //>=, not <=
		    if (scroll >= 300) {
		        //clearHeader, not clearheader - caps H
		        $(".site-header.cdb-header-fixed").addClass("scrolled");
		    }
				else {
        $(".site-header.cdb-header-fixed").removeClass("scrolled");


    }
		});


		$(window).scroll(function() {
var scroll = $(window).scrollTop();

//>=, not <=
if (scroll >= 300) {
//clearHeader, not clearheader - caps H
$(".site-header.cdb-header-fixed-2").addClass("scrolled");
}
else {
$(".site-header.cdb-header-fixed-2").removeClass("scrolled");


}
});

            },

            /**
             * Main Navigation DropDown Ancestor
             */
            dropdwon_arrow: function () {
                $('.studiare-navigation > ul > li.menu-item-has-children').each(function(){
                    $(this).find('> a').append('<i class="fa fa-angle-down"></i>');
                });
            },

			/**
             * Mobile Navigation DropDown
             */

			dropdwon_arrow_mobile: function() {

				$( ".off-canvas-navigation ul.sub-menu" ).before( "<i class='sub-menu-arrow fa fa-angle-left'></a>" );
				$( ".off-canvas-navigation .sub-menu-arrow" ).click(function() {
	            if($(this).hasClass("fa-angle-left")) {
	            	$(this).next("ul.sub-menu").show(500);
	            	$(this).removeClass("fa-angle-left").addClass("fa-angle-down");
	            }
	            else {
	            	$(this).next("ul.sub-menu").hide(500);
	            	$(this).removeClass("fa-angle-down").addClass("fa-angle-left");
	            }


	        });

			},


			dropdwon_arrow_sidebar: function() {

				$( ".sidebar-widgets-wrapper .widget_nav_menu ul>li" ).click(function() {
				if($(this).hasClass("menu-item-has-children")) {
	            	$(this).toggleClass("opened");
	            }
	        });
			},




            /**
             * Back to top
             */
            back_to_top: function() {
                var back_to_top = $('#back-to-top');

                $(window).scroll(function () {
                    if ($(this).scrollTop() > 100) {
                        back_to_top.addClass('visible');
                    } else {
                        back_to_top.removeClass('visible');
                    }
                });

                back_to_top.on('click', function (ev) {
                    ev.preventDefault();

                    $('html,body').animate({scrollTop: '0px'}, 800);
                })
            },

            /**
             * Off Canvas Navigation
             */
            off_canvas_navigation: function() {

                $('.mobile-nav-toggle').on('click', function(ev) {
                    ev.preventDefault();

                    body.toggleClass('off-canvas-open');
                });

                $('.off-canvas-overlay').on('click', function(ev) {
                    ev.preventDefault();

                    body.removeClass('off-canvas-open');
                });

            },

						/**
			 * Off Canvas My Account Navigation
			 */
			off_canvas_my_account_navigation: function() {

					$('.account-nav-toggle').on('click', function(ev) {
							ev.preventDefault();

							body.toggleClass('account-off-canvas-open');
					});

					$('.off-canvas-overlay').on('click', function(ev) {
							ev.preventDefault();

							body.removeClass('account-off-canvas-open');
					});

			},


			/**
             * Study Mode Btn
             */
            study_mode: function() {

                var course_content = $('.product-single-main');
				var course_side = $('.product-single-aside');
				$('.study-mode-btn').on('click', function(ev) {

                    course_content.toggleClass('full-width-course');
					course_side.toggleClass('hide-sidebar-course');
                });

            },



            /**
             * Login Form Modal
             */
            modal_login_form: function () {

                $('.register-modal-opener').on('click', function (e) {
                    e.preventDefault();
                    body.toggleClass('modal-login-open');
                });

                $('.login-form-overlay, .login-form-modal-box .close').on('click', function (e) {
                    e.preventDefault();
                    body.removeClass('modal-login-open')
                });

            },

			/**
             * Advice Form Modal
             */
            modal_advice_form: function () {

                $('.advice-modal-opener').on('click', function (e) {
                    e.preventDefault();
                    body.toggleClass('modal-advice-open');
                });

                $('.advice-form-overlay, .advice-modal-content .close').on('click', function (e) {
                    e.preventDefault();
                    body.removeClass('modal-advice-open')
                });

            },

            /**
             * Transform Select to Select2
             */
            select_to_select2: function () {
              $('select').select2({
                  width: '100%',
              })
            },

            /**
             * Courses Layout Swtich
             */
            courses_layout_switch: function () {
                var grid_class = 'grid-view',
                    list_class = 'list-view';

                var listSwitcher = function () {
                    var switcher_active = 'active';

                    $('.switcher-view-grid').on('click', function (ev) {
                        switchToGrid();
                        ev.preventDefault();
                    });

                    $('.switcher-view-list').on('click', function (ev) {
                        switchToList();
                        ev.preventDefault();
                    });

                    function switchToList() {
                        $('.switcher-view-list').addClass(switcher_active);
                        $('.switcher-view-grid').removeClass(switcher_active);
                        $('.products').fadeOut(300, function () {
                            $(this).removeClass(grid_class).addClass(list_class).fadeIn(300);
                        });
                    }

                    function switchToGrid() {
                        $('.switcher-view-grid').addClass(switcher_active);
                        $('.switcher-view-list').removeClass(switcher_active);
                        $('.products').fadeOut(300, function () {
                            $(this).removeClass(list_class).addClass(grid_class).fadeIn(300);
                        });
                    }

                };

                listSwitcher();

            },

            /**
             * Header Mini Cart
             */
            header_mini_cart: function () {
              var miniCartOpener = $('.mini-cart-opener');

              miniCartOpener.on('click', function (ev) {

                  ev.preventDefault();

                  $('.dropdown-cart').toggleClass('visible');

                  if($('.dropdown-cart').hasClass('visible'))
                  {
                      setTimeout(function()
                      {
                          $(document).on('click', closeMiniCartClickOutSide);
                      }, 1);
                  }
                  else
                  {
                      $(document).off('click', closeMiniCartClickOutSide);
                  }
              });

              var closeMiniCartClickOutSide = function (ev) {
                  if( ! $(ev.target).closest($('.dropdown-cart')).length) {
                      $('.dropdown-cart').removeClass('visible');
                      $(document).off('click', closeMiniCartClickOutSide);
                  }
              }

            },

						/**
			 * DropDown Menu
			 */
			dropdown_menu: function() {

					$('.header__details-user').on('click', function(ev) {
							ev.preventDefault();

							$('.header__details-user').toggleClass('user-menu-open');
							$('.user-menu__list').toggleClass('list-open');
					});

			},

            /**
             * Sticky Sidebar
             */
            sticky_sidebar: function () {

                var offsetTop = 30;
                var headerstick = 50;
								var headerstick2 = 90;


                if ($("body.fixed-body").length) {
                    offsetTop += headerstick + $("#wpadminbar").outerHeight();
                }

								if ($("body.fixed-body-2").length) {
                    offsetTop += headerstick2 + $("#wpadminbar").outerHeight();
                }



                if ($('.sticky-sidebar').length > 0) {
                    $(".sticky-sidebar").theiaStickySidebar({
                        "containerSelector"     : "",
                        "additionalMarginTop"   : offsetTop,
                        "additionalMarginBottom": "0",
                        "updateSidebarHeight"   : false,
                        "minWidth"              : "768",
                        "sidebarBehavior"       : "modern"
                    });
                }

            },

            /**
             * Video Button with Magnific Popup
             */
//             video_popup: function () {
//                 $(".cdb-video-icon, .video-lesson-preview").magnificPopup({
//                     type: 'iframe',
//                 });
//             },

            /**
             * Portfolio Filter
             */
            portfolioFilter: function () {

                $('.portfolio-controls .control').on('click', function (ev) {
                   ev.preventDefault();
                });

                if ( $('.portfolio-holder').length ) {
                    var mixer = mixitup('.portfolio-holder', {
                        selectors: {
                            "target": '.portfolio-entry'
                        },
                        animation: {
                            "duration": 250,
                            "nudge": true,
                            "reverseOut": false,
                            "effects": "fade stagger(100ms)"
                        }
                    });
                }
            },

            /**
             * Animated Counter
             */
            animatedCounter: function () {

                var counters = $('.counter-number');

                if (counters.length) {
                    counters.each(function () {
                        var counter = $(this);
                        counter.appear(function () {
                            counter.parent().css({'opacity': 1});

                            //Counter zero type
                            var max = parseFloat(counter.text());
                            counter.countTo({
                                from: 0,
                                to: max,
                                speed: 1500,
                                refreshInterval: 100
                            });

                        }, {accX: 0, accY: 0});
                    });
                }
            },

            /**
             * Course Categories
             */
            courseCategories: function () {

                var $course_grid = $('.course-categories').packery();

                $course_grid.imagesLoaded().progress( function() {
                    $course_grid.packery();
                });
            },

            /**
             * Blog Masonry
             */
            blogMasonry: function () {
                var $post_items = $('.blog-masonry').packery();


                $post_items.imagesLoaded().progress( function() {
                    $post_items.packery();
                });

            },

            /**
             * Testimonials Carousel
             */
            testimonialsCarousel: function () {
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
            },

            /**
             * Course Panel Toggle
             */
            coursePanel: function () {
                var acc = document.getElementsByClassName("course-panel-heading");
                var i;

                for (i = 0; i < acc.length; i++) {
                    acc[i].addEventListener("click", function() {
                        this.classList.toggle("active");
                        var panel = this.nextElementSibling;
                        if (panel.style.maxHeight){
                            panel.style.maxHeight = null;
                        } else {
                            panel.style.maxHeight = panel.scrollHeight + "px";
                        }
                    });
                }
            },

            /**
             * Count Down Timer
             */
            countDownTimer: function () {
                $('.countdown-item').each(function(){
                    $(this).countdown($(this).data('date'), function(event) {
                        $(this).html(event.strftime(''
                            + '<div class="countdown-col"><span class="countdown-unit countdown-days"><span class="number">%-D </span><span class="text">' + studiare_options.countdown_days + '</span></span></div> '
                            + '<div class="countdown-col"><span class="countdown-unit countdown-hours"><span class="number">%H </span><span class="text">' + studiare_options.countdown_hours + '</span></span></div> '
                            + '<div class="countdown-col"><span class="countdown-unit countdown-min"><span class="number">%M </span><span class="text">' + studiare_options.countdown_mins + '</span></span></div> '
                            + '<div class="countdown-col"><span class="countdown-unit countdown-sec"><span class="number">%S </span><span class="text">' + studiare_options.countdown_sec + '</span></span></div>'));
                    });
                })
            },

            /**
             * Gallery LightBox
             */
            galleryLightbox: function () {
                var galleryWrapper = $('.gallery-wrapper');

                galleryWrapper.each( function () {
                    var _this = $(this);

                    _this.magnificPopup({
                        mainClass: 'mfp-zoom-in',
                        type: 'image',
                        delegate: 'a.gallery-lightbox-link',
                        removalDelay: 400,
                        gallery: {
                            enabled:true
                        }
                    });
                });
            },

            /**
             * Gallery Carousel
             */
						 galleryCarousel: function () {
                 var carousel = $('.gallery-wrapper .owl-carousel');

                 if ( carousel.length ) {

                     carousel.each( function() {
                         var owl = $(this),
                             autoplay = true,
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
                             loop: loop,

                             onRefreshed: function() {
                                 $(window).resize();
                             }
                         });
                     });

                 }

             },


            /**
             * Courses Carousel
             */
            coursesCarousel: function () {
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

            },


            /**
             * Blog posts Carousel
             */
            blogpostsCarousel: function () {
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

            },


            /**
             * Megamenu Position
             */
            megamenupostion: function () {

              //*******************************************************************
  //* Megamenu windows exist
  //*******************************************************************/

  // position mega menu correctly
  jQuery.fn.emallshop_position_megamenu = function( variables ) {

    // top header headnling
    var reference_elem = '';
    reference_elem = jQuery( this ).parent( '.studiare-navigation' );

    if( jQuery( this ).parent( '.studiare-navigation' ).length ) {

      var main_nav_container = reference_elem,
        main_nav_container_position = main_nav_container.offset(),
        main_nav_container_width = main_nav_container.width(),
        main_nav_container_left_edge = main_nav_container_position.left,
        main_nav_container_right_edge = main_nav_container_left_edge + main_nav_container_width;

      if( ! jQuery( 'body.rtl' ).length ) {
        return this.each( function() {


        });

      } else {
        return this.each( function() {

          jQuery( this ).children( 'li' ).each( function() {
            var li_item = jQuery( this ),
              li_item_position = li_item.offset(),
              megamenu_wrapper = li_item.find( '.emallshop-megamenu-wrapper' ),
              megamenu_wrapper_width = megamenu_wrapper.outerWidth(),
              megamenu_wrapper_position = 0;

            // check if there is a megamenu
            if( megamenu_wrapper.length ) {
              megamenu_wrapper.removeAttr( 'style' );

              // reset the megmenu width after resizing the menu
              megamenu_wrapper_width = megamenu_wrapper.outerWidth();

              if( li_item_position.left + megamenu_wrapper_width > main_nav_container_right_edge ) {
                megamenu_wrapper_position = -1 * ( li_item_position.left - ( main_nav_container_right_edge - megamenu_wrapper_width ) );

                megamenu_wrapper.css( 'left', megamenu_wrapper_position );
              }
            }
          });
          jQuery( this ).children( 'li' ).each( function() {
            var li_item = jQuery( this ),
              li_item_position = li_item.offset(),
              li_item_right_edge = li_item_position.left + li_item.outerWidth(),
              megamenu_wrapper = li_item.find( '.emallshop-megamenu-wrapper' ),
              megamenu_wrapper_width = megamenu_wrapper.outerWidth(),
              megamenu_wrapper_position = 0;

            // check if there is a megamenu
            if( megamenu_wrapper.length ) {
              megamenu_wrapper.removeAttr( 'style' );

              // set megamenu max width
              var reference_emallshop_row;

              if( jQuery( '.emallshop-secondary-main-menu' ).length ) {
                reference_emallshop_row = jQuery( '.emallshop-header-wrapper .emallshop-secondary-main-menu .emallshop-row' );
              } else {
                reference_emallshop_row = jQuery( '.emallshop-header-wrapper .emallshop-row' );
              }

              if( megamenu_wrapper.hasClass( 'col-span-12' ) && ( reference_emallshop_row.width() < megamenu_wrapper.data( 'maxwidth' ) ) ) {
                megamenu_wrapper.css( 'width', reference_emallshop_row.width() );
              } else {
                megamenu_wrapper.removeAttr( 'style' );
              }

              if( li_item_right_edge - megamenu_wrapper_width < main_nav_container_left_edge ) {

                megamenu_wrapper_position = -1 * ( megamenu_wrapper_width - ( li_item_right_edge - main_nav_container_left_edge ) );

                megamenu_wrapper.css( 'left', megamenu_wrapper_position );
              }
            }
          });
        });
      }
    }
  };



            },

			/**
             * Login Register Froms
             */
            log_reg: function () {

				$(".login-btn").click(function(){
					$(".stu-reg").show();
					$(".stu-login").hide();
				});

				$(".reg-btn").click(function(){
					$(".stu-login").show();
					$(".stu-reg").hide();
				});

            },


						/**
										 * Shwo Box Download
										 */
								box_download: function () {

									$('.box_download span').on('click', function(){
											$('.box_download .box_content').slideToggle(400);
									});

									$('a.link-not').on('click', function(){
											$('.collapse').slideToggle(400);
									});

								},



        }
    }());

})(jQuery);

jQuery(document).ready(function($) {

	$('.video-button a').click(function(event){
		event.preventDefault();
		var post_id = $(this).attr('data-post-id');
		var url = $(this).attr('href');

		$('.video_popup_wrrapper').fadeIn();
		$('body').find('.video_popup_wrrapper .video_popup_inner').html('<div class="spinner"> <div class="double-bounce1"></div> <div class="double-bounce2"></div></div>');

		$.ajax({
    type: 'post',
    url:woocommerce_params['ajax_url'],
    data:{'action':'get_video_ajax','post_id':post_id,'url':url},

   success:function (response) {
      $('body').find('.video_popup_wrrapper .video_popup_inner').html('<video controls="" autoplay="" name="media"><source src="'+response+'" type="video/mp4"></video>');
	   $('.video_popup_wrrapper').fadeIn();
   }


});
});
	$('.video_popup_overlay').click(function(event){
		$('.video_popup_wrrapper').fadeOut();
		$('body').find('.video_popup_wrrapper .video_popup_inner video').remove();
	});
});


jQuery(document).ready(function($) {

	$('.panel-heading-right a.preview-button').click(function(event){
		event.preventDefault();
		var post_id = $(this).attr('data-lesson-id');
		var url = $(this).attr('href');

		$('.video_popup_wrrapper').fadeIn();
		$('body').find('.video_popup_wrrapper .video_popup_inner').html('<div class="spinner"> <div class="double-bounce1"></div> <div class="double-bounce2"></div></div>');

		$.ajax({
    type: 'post',
    url:woocommerce_params['ajax_url'],
    data:{'action':'get_lesson_video_ajax','post_id':post_id,'url':url},

   success:function (response) {
      $('body').find('.video_popup_wrrapper .video_popup_inner').html('<video controls="" autoplay="" name="media"><source src="'+response+'" type="video/mp4"></video>');
	   $('.video_popup_wrrapper').fadeIn();
   }


});
});
	$('.video_popup_overlay').click(function(event){
		$('.video_popup_wrrapper').fadeOut();
		$('body').find('.video_popup_wrrapper .video_popup_inner video').remove();
	});
});

jQuery(document).ready(function($) {

	$('a.testimonial-video').click(function(event){
		event.preventDefault();
		var post_id = $(this).attr('data-lesson-id');
		var url = $(this).attr('href');

		$('.video_popup_wrrapper').fadeIn();
		$('body').find('.video_popup_wrrapper .video_popup_inner').html('<div class="spinner"> <div class="double-bounce1"></div> <div class="double-bounce2"></div></div>');

		$.ajax({
    type: 'post',
    url:woocommerce_params['ajax_url'],
    data:{'action':'get_lesson_video_ajax','post_id':post_id,'url':url},

   success:function (response) {
      $('body').find('.video_popup_wrrapper .video_popup_inner').html('<video controls="" autoplay="" name="media"><source src="'+response+'" type="video/mp4"></video>');
	   $('.video_popup_wrrapper').fadeIn();
   }


});
});
	$('.video_popup_overlay').click(function(event){
		$('.video_popup_wrrapper').fadeOut();
		$('body').find('.video_popup_wrrapper .video_popup_inner video').remove();
	});
});


jQuery(document).ready(function($) {
    studiareTheme.init();
});
