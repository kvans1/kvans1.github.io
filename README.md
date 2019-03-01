# kvans1.github.io
<html>
  <head>my head</head>
</html>
<sql>
  -- phpMyAdmin SQL Dump
  -- version 4.8.3
  -- https://www.phpmyadmin.net/
  --
  -- Host: 127.0.0.1:3306
  -- Generation Time: Mar 01, 2019 at 01:10 AM
  -- Server version: 5.7.23
  -- PHP Version: 7.2.10

  SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
  SET AUTOCOMMIT = 0;
  START TRANSACTION;
  SET time_zone = "+00:00";


  /*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
  /*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
  /*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
  /*!40101 SET NAMES utf8mb4 */;

  --
  -- Database: `testdb`
  --

  -- --------------------------------------------------------

  --
  -- Table structure for table `students`
  --

  DROP TABLE IF EXISTS `students`;
  CREATE TABLE IF NOT EXISTS `students` (
    `StudentsID` int(11) NOT NULL AUTO_INCREMENT,
    `StudentFirstName` varchar(45) DEFAULT NULL,
    `StudentLastName` varchar(45) DEFAULT NULL,
    `StudentAge` int(11) DEFAULT NULL,
    PRIMARY KEY (`StudentsID`),
    UNIQUE KEY `StudentsID_UNIQUE` (`StudentsID`)
  ) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=latin1;

  --
  -- Dumping data for table `students`
  --

  INSERT INTO `students` (`StudentsID`, `StudentFirstName`, `StudentLastName`, `StudentAge`) VALUES
  (1, 'Kyle', 'Van Schaik', 16),
  (2, 'test', 'name', 19),
  (3, 'sham', 'bam', 16),
  (4, 'fkfsdk', '322323', 87),
  (5, 'fudge', 'serp', 69);
  COMMIT;

  /*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
  /*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
  /*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
</sql>
