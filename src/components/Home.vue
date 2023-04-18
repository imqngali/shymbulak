<template>
  <header class="header">
    <div class="nav">
        <div class="logo"><img src="../assets/img/logo.webp"></div>
        <div class="live">
			<img src="../assets/img/Live.webp">
		</div>
        <div class="weather">
			<img src="../assets/img/carusel-cloud.webp">
			<span>{{Math.round(currentData['main']['temp'] - 275)}}C°</span>
		</div>
        <div class="switcher"><img src="../assets/img/switcher.webp"></div>
        <div class="search"><img src="../assets/img/Search.webp"></div>
    </div>
    <div class="user">
        <div class="lang"><img src="../assets/img/Language.webp" alt=""></div>
        <div class="profile"><img src="../assets/img/Profile.webp" alt=""></div>
        <div class="saved"><img src="../assets/img/Saved.webp" alt=""></div>
        <div class="cart"><img src="../assets/img/Cart.webp" alt=""></div>
    </div>
</header>

	<main class="main">
		<div class="container">
			<h1 class="main__title">Погода</h1>
			<div class="weather_board">
				<div class="weather_board__now">
					<div>
						<h2 class="weather_board__now__title">Сейчас</h2>
						<img class="weather_board__now__state" src="../assets/img/cloudy.webp" alt="">
					</div>	
					<div class="weather_board__now__text">
						<h3 class="weather_board__now__text__title">Облачно</h3>
						<h1 class="weather_board__now__text__degree">{{Math.round(currentData['main']['temp'] - 275)}}°C</h1>
						<div class="weather_board__now__text__line"></div>
						<div class="weather_board__now__text__additional">
							<div>
								<img src="../assets/img/wind.webp" alt="">
								<span>{{Math.round(currentData['wind']['speed'])}} м/c</span>
							</div>
							<div>
								<img src="../assets/img/blob.webp" alt="">
								<span>"{{Math.round(currentData['main']['humidity'])}} "см</span>
							</div>
						</div>
					</div>
					
				</div>
				<div class="weather_board__day">
					<h1 class="weather_board__day__title">Погода в течении дня</h1>
					<div class="weather_board__day__line"></div>
					<div class="weather_board__day__carusel">
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
						<div class="weather_board__day__carusel__block">
							<h5 class="weather_board__day__carusel__block__title">01</h5>
							<img class="weather_board__day__carusel__block__img" src="../assets/img/carusel-cloud.png">
							<h2 class="weather_board__day__carusel__block__degree">26°</h2>
						</div>
					</div>
				</div>
			</div>
			<div class="week">
				<h1 class="week__title">Прогноз на 10 дней</h1>
				<div class="week__days">
					<div class="week__days_day">
						<h3 class="week__days_day__title">Сегодня</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
					<div class="week__days_day">
						<h3 class="week__days_day__title">ПН</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
					<div class="week__days_day">
						<h3 class="week__days_day__title">ВТ</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
					<div class="week__days_day">
						<h3 class="week__days_day__title">СР</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
					<div class="week__days_day">
						<h3 class="week__days_day__title">ЧТ</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
					<div class="week__days_day">
						<h3 class="week__days_day__title">ПТ</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
					<div class="week__days_day">
						<h3 class="week__days_day__title">СБ</h3>
						<span class="week__days_day__date">11 июля</span>
						<img class="week__days_day__img" src="../assets/img/week-w.png" alt="">
						<span class="week__days_day__speed">мин. <b>16°</b></span>
						<span class="week__days_day__max-speed">макс. <b>28°</b></span>
					</div>
				</div>
			</div>
		</div>
	</main>
	<footer class="footer">
    <div class="container">
        <div class="footer__inner">
            <div class="footer__inner__apps">
                <img class="footer__inner__apps__logo" src="../assets/img/footer-logo.png" alt="">
                <img src="../assets/img/googleplay.png" alt="" class="footer__inner__apps__google-play">
                <img src="../assets/img/appstore.png" alt="" class="footer__inner__apps__app-store">
            </div>
            <div class="footer__inner__nav">
                <div class="footer__inner__nav__resort">
                    <h2 class="footer__inner__nav__resort__title">Курорт</h2>
                    <div class="footer__inner__nav__resort__nav">
                        <nav class="footer__inner__nav__resort__nav__item">Отели</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Рестораны</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Развлечения</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Магазин</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Детям</nav>
                    </div>
                </div>
                <div class="footer__inner__nav__activity">
                    <h2 class="footer__inner__nav__activity__title">Катания</h2>
                    <div class="footer__inner__nav__activity__nav">
                        <nav class="footer__inner__nav__activity__nav__item">Билеты</nav>
                        <nav class="footer__inner__nav__activity__nav__item">Прокат</nav>
                        <nav class="footer__inner__nav__activity__nav__item">Школа</nav>
                        <nav class="footer__inner__nav__activity__nav__item">Паркинг</nav>
                    </div>
                </div>
                <div class="footer__inner__nav__info">
                    <h2 class="footer__inner__nav__resort__title">Инфо</h2>
                    <div class="footer__inner__nav__resort__nav">
                        <nav class="footer__inner__nav__resort__nav__item">Погода</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Правила</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Новости</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Как добраться</nav>
                        <nav class="footer__inner__nav__resort__nav__item">Тех. поддержка</nav>
                    </div>
                </div>
                <div class="footer__inner__nav__contacts">
                    <h2 class="footer__inner__nav__contacts__title">Контакты</h2>
                    <div class="footer__inner__nav__contacts__social">
                        <img src="../assets/img/facebook.png" alt="">
                        <img src="../assets/img/youtube.png" alt="">
                        <img src="../assets/img/instagram.png" alt="">
                        <img src="../assets/img/vk.png" alt="">
                    </div>
                    <div class="footer__inner__nav__contacts__nav">
                        <nav class="footer__inner__nav__contacts__nav__item">info@shymbulak.com</nav>
                        <nav class="footer__inner__nav__contacts__nav__item">+7 727 331 77 77</nav>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer__line"></div>
        <div class="footer__copyrights">
            <h4>© 2022 ТОО «Chimbulak Development»</h4>
            <h4>created by YOKO</h4>
        </div>
    </div>
</footer>
</template>

<script>

export default {
  name: 'Home-page',
  props: {
    currentData: Object
  }
}
</script>

