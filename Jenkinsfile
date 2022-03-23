// Declarativa: Es mas comoda... mas guiada... menos flexible
pipeline {
    
    agent any;
    
    stages {
        stage('Compilacion'){
            steps {
                echo 'Compilar'
                echo 'Estoy en ello'
                echo 'Listo'
            }
            post {
                succes{
                     echo 'Se ejecuta solo si los steps han ido bien'
                }
                failure{
                    echo 'Se ejecuta solo si los steps han ido mal'
                }
                always{
                    echo 'Se ejecuta siempre'
                }
            }
        }
        stage('Pruebas'){
            steps {
                echo 'Voy a Probar'
                echo 'Estoy en ello'
                echo 'Listo'
            }
            post {
                succes{
                     echo 'Se ejecuta solo si los steps han ido bien'
                }
                failure{
                    echo 'Se ejecuta solo si los steps han ido mal'
                }
                always{
                    echo 'Se ejecuta siempre'
                }
            }
        }
    }
    
    // Tanto la marca post, como las marcas de dentro son opcionales
    post {
        succes{
             echo 'Se ejecuta solo si los stages han ido bien'
        }
        failure{
            echo 'Se ejecuta solo si los stages han ido mal'
        }
    }
}

// Scripted: Es mas potente, mas flexible... menos comoda (LA BUENA)