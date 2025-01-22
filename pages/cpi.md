# Relationship Between CPI, Labor Force Characteristics and Opioid Deaths in Canada

This project was created by myself, Bobbi Boyce, Kennedy Gunderson and  Noah Seminoff. 

All of the analysis was completed using Python.

Libraries used: Pandas, Numpy, Datetime, Sqlalchemy, Matplotlib, Plotly and Statsmodels

The entire project report can be found [HERE](https://maxwellpaterson.github.io/projects/Data604_Final_Report.html)

### Goal

The goal of this project was to take four datasets and create a data model to connect them all together so that analysis using multiple datasources at once was possible. This was an introduction to data modelling and how to use primary and foreign keys to connect data bases together correctly. We also implemented the use of SQL in order to join and pull data from the tables we were using.

### Process

""SQL("""
    select Region_Year_Quarter,
    cast(Total_opioid_toxicity_deaths as int) as Total_opioid_toxicity_deaths
    from Opiates
    where region != 'Territories'
        and region != 'Whitehorse, Yukon'
        and region != 'Winnipeg, Manitoba'
        and region != 'Yellowknife, Northwest Territories'
        and region != 'Northern and rural Manitoba'
        and region != 'Canada'
        and Total_opioid_toxicity_deaths > (select avg(Total_opioid_toxicity_deaths) from Opiates
                                            where region != 'Territories'
                                            and region != 'Whitehorse, Yukon'
                                            and region != 'Winnipeg, Manitoba'
                                            and region != 'Yellowknife, Northwest Territories'
                                            and region != 'Northern and rural Manitoba'
                                            and region != 'Canada')
    group by Total_opioid_toxicity_deaths desc
    """)""

### Conclusion


