## CURRICULUM VITAE

**Nombre:** {{ site.data.cv.nombre }}

**Formación académica:** {{ site.data.cv.formacion }}

<img src= "https://tmssl.akamaized.net/images/foto/normal/lionel-messi-ballon-dor-2019-1592819026-41968.jpg" />

**Enlace:** [GitHub Pages](https://pages.github.com/)

**Mis aficiones son:**
{% for aficion in site.data.cv.aficiones -%} 
* {{ aficion.deporte }}
* {{ aficion.musica }}
* {{ aficion.serie }}
{% endfor %} 

**Cita preferida:**
> {{ site.data.cv.cita }}

**Código:**

    if imag(solucion(:,1))~=0 %para no tener en cuenta valores de potencia que hagan todas las soluciones complejas
        continue
    else
        sol_reales=[]; %para reiniciar la variable en cada iteración
        for i=1:4    
            solucion(i);
            if solucion(i)>=0
               sol_reales=[sol_reales,solucion(i)];
            end
        end
        U2_estable=[max(sol_reales)]; %solución estable de la ecuación
        U2_inestable=[min(sol_reales)]; %solución inestable de la ecuación
        Upcc_estable=[Upcc_estable,U2_estable];
        Upcc_inestable=[Upcc_inestable,U2_inestable];
        P_sol=[P_sol,P]; %valores de P válidos
    end

<span style='font-size:100px;'>&#8986;</span>

{% for lengua in site.data.cv.tabla -%} 
| Idioma | Nivel |
| ------------- | ------------- |
| {{ lengua.idioma }} | {{ lengua.nivel }} |
{% endfor %} 
