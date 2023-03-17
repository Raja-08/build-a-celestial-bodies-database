--
-- PostgreSQL database dump
--

-- Dumped from database version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
-- Dumped by pg_dump version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    galaxy_id integer NOT NULL,
    nostars integer,
    nosun integer,
    weight numeric(4,1),
    farearth boolean,
    farmoon boolean,
    location text,
    name character varying(20) NOT NULL
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: milkyway; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.milkyway (
    name character varying(20),
    location character varying(20) NOT NULL,
    type character varying(20) NOT NULL,
    milkyway_id integer NOT NULL
);


ALTER TABLE public.milkyway OWNER TO freecodecamp;

--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    moon_id integer NOT NULL,
    nostars integer,
    nosun integer,
    weight numeric(4,1),
    farearth boolean,
    farmoon boolean,
    location text,
    planet_id integer,
    name character varying(20) NOT NULL
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    planet_id integer NOT NULL,
    nostars integer,
    nosun integer,
    weight numeric(4,1),
    farearth boolean,
    farmoon boolean,
    location text,
    star_id integer,
    name character varying(20) NOT NULL
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    star_id integer NOT NULL,
    nostars integer,
    nosun integer,
    weight numeric(4,1),
    farearth boolean,
    farmoon boolean,
    location text,
    galaxy_id integer,
    name character varying(20) NOT NULL
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES (1, 2, 3, 45.3, true, false, 'Earth', 'Madurai');
INSERT INTO public.galaxy VALUES (2, 4, 4, 45.3, true, false, 'Venus', 'Chennai');
INSERT INTO public.galaxy VALUES (3, 43, 14, 145.3, true, false, 'Mars', 'Chennai');
INSERT INTO public.galaxy VALUES (4, 4, 14, 135.3, true, false, 'Neptune', 'Chennai');
INSERT INTO public.galaxy VALUES (5, 4, 14, 235.3, true, false, 'Jupiter', 'Chennai');
INSERT INTO public.galaxy VALUES (6, 4, 14, 435.3, true, false, 'Saturn', 'Chennai');


--
-- Data for Name: milkyway; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.milkyway VALUES ('R', 'Ind', 'R', 1);
INSERT INTO public.milkyway VALUES ('Rt', 'Inda', 'Ra', 2);
INSERT INTO public.milkyway VALUES ('Rtr', 'Indan', 'Rja', 3);


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES (1, 2, 1, 141.0, true, false, 'IT', 1, 'Q');
INSERT INTO public.moon VALUES (2, 3, 1, 124.0, true, false, 'IAT', 2, 'P');
INSERT INTO public.moon VALUES (3, 5, 1, 122.0, true, false, 'TAI', 3, 'O');
INSERT INTO public.moon VALUES (4, 8, 1, 622.0, false, false, 'HK', 4, 'K');
INSERT INTO public.moon VALUES (5, 8, 1, 722.0, false, false, 'H', 5, 'J');
INSERT INTO public.moon VALUES (6, 8, 1, 722.0, false, false, 'ICE', 6, 'I');
INSERT INTO public.moon VALUES (7, 3, 1, 522.0, false, true, 'UAE', 7, 'H');
INSERT INTO public.moon VALUES (8, 5, 1, 520.0, false, true, 'AUS', 8, 'G');
INSERT INTO public.moon VALUES (9, 8, 1, 120.0, false, false, 'AU', 9, 'R');
INSERT INTO public.moon VALUES (10, 18, 1, 420.0, true, false, 'UU', 10, 'U');
INSERT INTO public.moon VALUES (11, 8, 1, 620.0, true, false, 'UUT', 11, 'UR');
INSERT INTO public.moon VALUES (12, 64, 1, 62.0, true, false, 'U', 12, 'URN');
INSERT INTO public.moon VALUES (13, 64, 14, 624.0, true, true, 'UT', 1, 'URNQ');
INSERT INTO public.moon VALUES (14, 64, 14, 624.0, true, true, 'UTA', 1, 'URNQ');
INSERT INTO public.moon VALUES (15, 64, 14, 624.0, true, true, 'URE', 1, 'URNA');
INSERT INTO public.moon VALUES (16, 64, 14, 624.0, true, true, 'UETE', 1, 'U');
INSERT INTO public.moon VALUES (17, 64, 14, 624.0, true, true, 'FARE', 1, 'U');
INSERT INTO public.moon VALUES (18, 64, 14, 624.0, true, true, 'FAR', 1, 'U');
INSERT INTO public.moon VALUES (19, 64, 14, 624.0, true, true, 'FRAR', 2, 'AGU');
INSERT INTO public.moon VALUES (20, 4, 1, 654.0, true, false, 'FRHR', 8, 'AFT');


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES (1, 2, 1, 341.2, true, true, 'Ind', 1, 'L');
INSERT INTO public.planet VALUES (2, 2, 1, 141.2, false, false, 'China', 2, 'K');
INSERT INTO public.planet VALUES (3, 1, 1, 241.2, false, true, 'Kenya', 3, 'A');
INSERT INTO public.planet VALUES (4, 5, 1, 641.2, false, true, 'SWZ', 4, 'O');
INSERT INTO public.planet VALUES (5, 6, 1, 841.2, false, false, 'UAE', 5, 'P');
INSERT INTO public.planet VALUES (6, 3, 1, 941.2, true, true, 'DUBAI', 5, 'J');
INSERT INTO public.planet VALUES (7, 3, 1, 441.2, false, true, 'ARAB', 6, 'J');
INSERT INTO public.planet VALUES (8, 3, 1, 411.2, false, false, 'RUS', 3, 'E');
INSERT INTO public.planet VALUES (9, 3, 1, 401.2, false, true, 'FRA', 3, 'D');
INSERT INTO public.planet VALUES (10, 3, 1, 451.2, true, true, 'BEL', 2, 'C');
INSERT INTO public.planet VALUES (11, 3, 1, 471.2, true, false, 'ANT', 1, 'T');
INSERT INTO public.planet VALUES (12, 7, 1, 271.2, true, false, 'AUS', 1, 'G');


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES (1, 2, 1, 43.2, true, false, 'India', 1, 'R');
INSERT INTO public.star VALUES (2, 2, 1, 43.2, true, false, 'Ind', 2, 'S');
INSERT INTO public.star VALUES (3, 4, 1, 143.2, true, true, 'PAK', 3, 'K');
INSERT INTO public.star VALUES (4, 4, 1, 143.2, true, true, 'USA', 4, 'D');
INSERT INTO public.star VALUES (5, 4, 1, 143.2, true, true, 'UK', 4, 'D');
INSERT INTO public.star VALUES (6, 4, 1, 143.2, true, true, 'HK', 4, 'D');


--
-- Name: galaxy galaxy_location_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_location_key UNIQUE (location);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: milkyway milkyway_location_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.milkyway
    ADD CONSTRAINT milkyway_location_key UNIQUE (location);


--
-- Name: milkyway milkyway_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.milkyway
    ADD CONSTRAINT milkyway_pkey PRIMARY KEY (milkyway_id);


--
-- Name: moon moon_location_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_location_key UNIQUE (location);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: planet planet_location_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_location_key UNIQUE (location);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_location_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_location_key UNIQUE (location);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: moon moon_planet_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_planet_id_fkey FOREIGN KEY (planet_id) REFERENCES public.planet(planet_id);


--
-- Name: planet planet_star_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_star_id_fkey FOREIGN KEY (star_id) REFERENCES public.star(star_id);


--
-- Name: star star_galaxy_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_galaxy_id_fkey FOREIGN KEY (galaxy_id) REFERENCES public.galaxy(galaxy_id);


--
-- PostgreSQL database dump complete
--

