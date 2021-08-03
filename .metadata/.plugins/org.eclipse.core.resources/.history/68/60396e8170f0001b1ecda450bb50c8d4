package com.example.aop;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.CommandLineRunner;
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.context.ApplicationContext;
import org.springframework.context.annotation.Bean;

import com.example.aop.service.EmployeeManager;

@SpringBootApplication
public class AopLoggingApplication {

	@Autowired
	private EmployeeManager employeeManager;

	public static void main(String[] args) {
		SpringApplication.run(AopLoggingApplication.class, args);
	}

	@Bean
	public CommandLineRunner commandLineRunner(ApplicationContext ctx) {
		return args -> {

			System.out.println(employeeManager.getEmployeeById(1L));

		};
	}

}
