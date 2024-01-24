# Rtrend Forecast – Glossary

## Terms

- Aggregated (data) = relative to the lower time resolution. Aggregated from _granular_ data.
- (Forecast) Context = a set of circumstances and procedures that concretely define how the forecast is performed.
 In the code, a context is defined as a subclass of `Forecast` (or `ForecastOperator`) and a configuration file. 
- Granular (data) = Relative to the higher time resolution, in which the forecast pipeline is performed. Opposes _aggregated_ data.
- Incidence = generic denomination for the quantity that's being forecast. E.g.: number of influenza hospitalizations.
- "(A) Forecast" = one execution of the forecast pipeline, along with its data.
- (Forecast) Stage = set of procedures in the forecast pipeline. E.g.: `preprocessing`, `rt_estimation`, `inc_reconstruction` are labels of forecast stages. 
- (Forecast) Step = each execution of a forecast stage. Stages may be executed non-sequentially (for example, after reconstruction, the operator may decide to return to rt_estimation); each of such execution is a step. Steps are counted sequentially. 
- Subject

## Variable prefixes/suffixes

- ar = Array (`numpy.ndarray`)
- df = DataFrame (`pandas.DataFrame`)
- ens = ensemble. A sequence of items realized from some statistical distribution (known or not).
- fore = related to the "future" (starting at pres).
- gra = Granular 
- idx = Index. Eiter a pandas `Index` and its subclasses, or a regular index.
- inc = incid = Incidence
- obj = Object. Refers to an instance of some internal class.
- past = related to the "past" (before pres).
- pres
- sr = Series (`pandas.Series`)


## Common indexes and mute variables

- `i_t` = integer index of a time period.
- `tlabel` = a pd.Timestamp label of a time period.

