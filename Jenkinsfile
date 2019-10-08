Pipeline {
agent any
Stages {
Stage ('SCM checkout') {
steps ('https://github.com/Deepti1103/maven-project.git') }
}

Stage ('Compile maven') {
Steps {
WithMaven (maven : MyMaven) {
sh 'maven complied'
}}}

Stage ('test maven') {
parallel {
Steps {
WithMaven (maven: MyMaven) {
sh 'unit testing maven'
}}
Steps {
WithMaven (maven: MyMaven) {
sh 'UAT for maven'
)))

Stage ('Package maven') {
Steps {
WithMaven (maven: MyMaven) {
sh 'package maven'
)))

Stage ('Install Maven') {

Steps {
input "do you want to install?"
WithMaven (maven: MyMaven) {
sh 'maven clean install'
}}}
