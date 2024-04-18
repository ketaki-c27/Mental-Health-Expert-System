import java.util.Scanner;
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static String[][] Symptom(int n) {
        String[][] ADHD_S = {
    {"Forgetfulness", "N"},
    {"Hyperactivity", "N"},
    {"Impulsivity", "N"},
    {"Inattention", "N"}};

String[][] AgoraphobiaS = {
    {"Avoidance of certain situations", "N"},
    {"Fear of being in places or situations", "N"},
    {"Panic or anxiety in feared situations", "N"},
    {"Physical symptoms (sweating, trembling)", "N"}};

String[][] Anorexia_NervosaS = {
    {"Intense fear of gaining weight", "N"},
    {"Distorted body image", "N"},
    {"Restriction of food intake", "N"},
    {"Significantly low body weight", "N"}
};

String[][] Antisocial_PersonalityS = {
    {"Persistent lying or deceit", "N"},
    {"Disregard for and violation of others' rights", "N"},
    {"Aggression or violence", "N"},
    {"Lack of remorse", "N"}
};

String[][] ASD_S = {
    {"Challenges with communication", "N"},
    {"Difficulty with social interaction", "N"},
    {"Restricted interests or repetitive behaviors", "N"},
    {"Sensory sensitivities", "N"}
};

String[][] Binge_EatingS = {
    {"Feeling out of control during binges", "N"},
    {"Eating much more rapidly than normal", "N"},
    {"Recurrent episodes of binge eating", "N"},
    {"Eating until uncomfortably full", "N"}
};

String[][] Bipolar_DisorderS = {
    {"Periods of elevated mood (mania)", "N"},
    {"Periods of depression", "N"},
    {"Increased energy during manic episodes", "N"},
    {"Impulsivity", "N"}
};

String[][] Borderline_PersonalityS = {
    {"Impulsive behavior", "N"},
    {"Intense fear of abandonment", "N"},
    {"Unstable relationships", "N"},
    {"Unstable self-image", "N"}
};

String[][] Bulimia_NervosaS = {
    {"Compensatory behaviors (e.g., vomiting)", "N"},
    {"Recurrent episodes of binge eating", "N"},
    {"Self-evaluation influenced by body shape", "N"},
    {"Weight-induced self-esteem", "N"}
};

String[][] Dependent_PersonalityS = {
    {"Excessive need to be taken care of", "N"},
    {"Difficulty making decisions", "N"},
    {"Fear of abandonment", "N"},
    {"Lack of self-confidence", "N"}
};

String[][] DepressionS = {
    {"Changes in appetite", "N"},
    {"Difficulty concentrating", "N"},
    {"Feelings of worthlessness", "N"},
    {"Persistent sadness", "N"}
};

String[][] Dissociative_IdentityS = {
    {"Depersonalization or derealization", "N"},
    {"Gaps in memory", "N"},
    {"Presence of two or more distinct personality states", "N"},
    {"Significant distress", "N"}
};

String[][] ExcoriationS = {
    {"Attempts to decrease or stop picking", "N"},
    {"Recurrent picking at one's skin", "N"},
    {"Skin lesions or scarring", "N"},
    {"Significant distress or impairment", "N"}
};

String[][] Generalized_AnxietyS = {
    {"Difficulty controlling worry", "N"},
    {"Excessive worry", "N"},
    {"Irritability", "N"},
    {"Muscle tension", "N"}
};

String[][] Hoarding_DisorderS = {
    {"Accumulation of a large number of possessions", "N"},
    {"Distress or impairment due to hoarding behavior", "N"},
    {"Persistent difficulty discarding possessions", "N"},
    {"Significant cluttering", "N"}
};

String[][] HypersomnolenceS = {
    {"Difficulty waking up", "N"},
    {"Excessive daytime sleepiness", "N"},
    {"Prolonged nighttime sleep", "N"},
    {"Sleep inertia", "N"}
};

String[][] InsomniaS = {
    {"Difficulty falling asleep", "N"},
    {"Impairment in daytime functioning", "N"},
    {"Non-restorative sleep", "N"},
    {"Waking up too early", "N"}
};

String[][] Intellectual_DisabilityS = {
    {"Below-average intellectual functioning", "N"},
    {"Deficits in adaptive functioning", "N"},
    {"Developmental onset", "N"},
    {"Significant limitations", "N"}
};

String[][] Narcissistic_PersonalityS = {
    {"Exploitative behavior", "N"},
    {"Grandiosity", "N"},
    {"Lack of empathy", "N"},
    {"Need for admiration", "N"}
};

String[][] Obsessive_CompulsiveS = {
    {"Compulsions", "N"},
    {"Excessive checking or cleaning", "N"},
    {"Fear of contamination", "N"},
    {"Obsessions", "N"}
};

String[][] Panic_DisorderS = {
    {"Chest pain", "N"},
    {"Fear of losing control", "N"},
    {"Palpitations", "N"},
    {"Sudden feelings of terror", "N"}
};

String[][] Paranoid_PersonalityS = {
    {"Distrust and suspicion", "N"},
    {"Reluctance to confide", "N"},
    {"Unjustified belief", "N"},
    {"Vindictiveness", "N"}
};

String[][] Post_TraumaticS = {
    {"Avoidance of reminders", "N"},
    {"Hyperarousal", "N"},
    {"Intrusive memories or flashbacks", "N"},
    {"Negative changes in mood", "N"}
};

String[][] Schizoid_PersonalityS = {
    {"Detachment from social relationships", "N"},
    {"Limited range of emotional expression", "N"},
    {"Preference for solitary activities", "N"},
    {"Uninterested in close relationships", "N"}
};

String[][] Schizotypal_PersonalityS = {
    {"Odd or eccentric behavior", "N"},
    {"Peculiar thoughts, beliefs, or perceptions", "N"},
    {"Social anxiety", "N"},
    {"Unusual perceptual experiences", "N"}
};

String[][] SchizophreniaS = {
    {"Delusions", "N"},
    {"Disorganized speech", "N"},
    {"Hallucinations", "N"},
    {"Reduced expression of emotions", "N"}
};

String[][] Social_AnxietyS = {
    {"Avoidance of social situations", "N"},
    {"Difficulty speaking", "N"},
    {"Fear of judgment", "N"},
    {"Intense fear of social situations", "N"}
};

String[][] Specific_LearningS = {
    {"Challenges with understanding", "N"},
    {"Difficulty learning", "N"},
    {"Reading, writing, or math difficulties", "N"},
    {"Recalling spoken language", "N"}
};

String[][] Specific_PhobiasS = {
    {"Avoidance of the feared object", "N"},
    {"Intense fear or anxiety", "N"},
    {"Panic or distress", "N"},
    {"Specific object or situation", "N"}
};

String[][] TrichotillomaniaS = {
    {"Recurrent pulling out of one's hair", "N"},
    {"Sense of tension or relief", "N"},
    {"Significant distress", "N"},
    {"Significant impairment", "N"}
};

        List<String[][]> Symptoms = new ArrayList<>();

        Symptoms.add(ADHD_S);
Symptoms.add(AgoraphobiaS);
Symptoms.add(Anorexia_NervosaS);
Symptoms.add(Antisocial_PersonalityS);
Symptoms.add(ASD_S);
Symptoms.add(Binge_EatingS);
Symptoms.add(Bipolar_DisorderS);
Symptoms.add(Borderline_PersonalityS);
Symptoms.add(Bulimia_NervosaS);
Symptoms.add(Dependent_PersonalityS);
Symptoms.add(DepressionS);
Symptoms.add(Dissociative_IdentityS);
Symptoms.add(ExcoriationS);
Symptoms.add(Generalized_AnxietyS);
Symptoms.add(Hoarding_DisorderS);
Symptoms.add(HypersomnolenceS);
Symptoms.add(InsomniaS);
Symptoms.add(Intellectual_DisabilityS);
Symptoms.add(Narcissistic_PersonalityS);
Symptoms.add(Obsessive_CompulsiveS);
Symptoms.add(Panic_DisorderS);
Symptoms.add(Paranoid_PersonalityS);
Symptoms.add(Post_TraumaticS);
Symptoms.add(Schizoid_PersonalityS);
Symptoms.add(Schizotypal_PersonalityS);
Symptoms.add(SchizophreniaS);
Symptoms.add(Social_AnxietyS);
Symptoms.add(Specific_LearningS);
Symptoms.add(Specific_PhobiasS);
Symptoms.add(TrichotillomaniaS);

        return Symptoms.get(n);
}

    public static String[] Cause(int n) {
        String[] ADHD_C = {
    "Genetic predisposition.",
    "Differences in brain structure and function, particularly involving areas related to attention and impulse control.",
    "Environmental factors such as prenatal exposure to toxins or early childhood trauma."
};

String[] AgoraphobiaC = {"Genetic predisposition.","Past experiences of trauma or stressful events.","Having a panic disorder or other anxiety disorder."};

String[] Anorexia_NervosaC = {
    "Genetic predisposition.",
    "Psychological factors such as low self-esteem or body image dissatisfaction.",
    "Cultural influences emphasizing thinness or dieting."
};

String[] Antisocial_PersonalityC = {
    "Genetic predisposition.",
    "Early childhood trauma or neglect.",
    "Lack of positive role models or supportive relationships."
};

String[] ASD_C = {
    "Genetic predisposition.",
    "Abnormalities in brain development, particularly involving areas related to social interaction and communication.",
    "Environmental factors such as prenatal exposure to toxins or maternal infection during pregnancy."
};

String[] Binge_EatingC = {
    "Genetic predisposition.",
    "Psychological factors such as stress, depression, or low self-esteem.",
    "Dieting or restrictive eating patterns."
};

String[] Bipolar_DisorderC = {
    "Genetic factors, as bipolar disorder tends to run in families.",
    "Neurochemical imbalances, involving neurotransmitters like serotonin, dopamine, and norepinephrine.",
    "Environmental triggers such as stressful life events or disruptions in sleep patterns."
};

String[] Borderline_PersonalityC = {
    "Genetic predisposition.",
    "Childhood trauma or neglect.",
    "Dysfunctional family dynamics or unstable relationships."
};

String[] Bulimia_NervosaC = {
    "Genetic predisposition.",
    "Psychological factors such as low self-esteem or negative body image.",
    "Sociocultural factors such as media portrayals of thinness or beauty standards."
};

String[] Dependent_PersonalityC = {
    "Genetic predisposition.",
    "Early experiences of abandonment or rejection.",
    "Overprotective or controlling parenting styles."
};

String[] DepressionC = {
    "Biological factors such as genetics, brain chemistry, and hormones.",
    "Environmental factors like trauma, stress, or loss.",
    "Psychological factors including negative thinking patterns and low self-esteem."
};

String[] Dissociative_IdentityC = {
    "Severe trauma during childhood, often involving physical or sexual abuse.",
    "Lack of supportive relationships or coping mechanisms.",
    "Vulnerability factors such as genetic predisposition or personality traits."
};

String[] ExcoriationC = {
    "Genetic predisposition.",
    "Psychological factors such as stress or anxiety.",
    "Environmental factors such as boredom or body-focused repetitive behaviors."
};

String[] Generalized_AnxietyC = {
    "Genetic predisposition to anxiety disorders.",
    "Brain chemistry imbalances, particularly involving neurotransmitters like serotonin and gamma-aminobutyric acid (GABA).",
    "Environmental stressors such as trauma, abuse, or significant life changes."
};

String[] Hoarding_DisorderC = {
    "Genetic predisposition.",
    "Traumatic experiences or losses.",
    "Other mental health disorders such as depression or anxiety."
};

String[] HypersomnolenceC = {
    "Genetic predisposition.",
    "Medical conditions such as sleep apnea or neurological disorders.",
    "Medications that affect sleep patterns."
};

String[] InsomniaC = {
    "Stressful life events or significant changes in routine.",
    "Medical conditions such as chronic pain or respiratory disorders.",
    "Mental health disorders such as anxiety or depression."
};

String[] Intellectual_DisabilityC = {
    "Genetic factors, including chromosomal abnormalities or inherited disorders.",
    "Prenatal exposure to toxins or infections.",
    "Complications during childbirth or early childhood injuries."
};

String[] Narcissistic_PersonalityC = {
    "Developmental factors, such as excessive praise or criticism during childhood.",
    "Genetic predisposition.",
    "Cultural or societal influences."
};

String[] Obsessive_CompulsiveC = {
    "Genetic predisposition.",
    "Abnormalities in brain structure and function, particularly involving areas related to decision-making and fear.",
    "Environmental factors such as trauma or stress."
};

String[] Panic_DisorderC = {
    "Genetic factors.",
    "Brain chemistry imbalances, particularly involving neurotransmitters like serotonin and norepinephrine.",
    "Major life stressors or traumatic events."
};

String[] Paranoid_PersonalityC = {
    "Genetic predisposition.",
    "Early childhood experiences such as neglect or abuse.",
    "Cultural or societal factors emphasizing distrust or suspicion."
};

String[] Post_TraumaticC = {
    "Direct exposure to a traumatic event.",
    "Individual factors such as genetic predisposition or personality traits.",
    "Lack of social support or coping mechanisms."
};

String[] SchizophreniaC = {
    "Genetic predisposition.",
    "Neurochemical imbalances, particularly involving dopamine and glutamate.",
    "Brain structure abnormalities, including enlarged ventricles or reduced gray matter."
};

String[] Schizoid_PersonalityC = {
    "Genetic predisposition.",
    "Early childhood experiences of emotional coldness or detachment.",
    "Cultural or societal factors emphasizing independence or self-sufficiency."
};

String[] Schizotypal_PersonalityC = {
    "Genetic predisposition.",
    "Abnormalities in brain structure and function, particularly involving areas related to perception and cognition.",
    "Childhood experiences of trauma or neglect."
};

String[] Social_AnxietyC = {
    "Genetic predisposition.",
    "Brain structure and function, particularly in areas related to fear and anxiety.",
    "Environmental factors such as traumatic experiences or learned behaviors."
};

String[] Specific_LearningC = {
    "Genetic predisposition.",
    "Differences in brain structure and function, particularly involving areas related to language processing or mathematical skills.",
    "Environmental factors such as early childhood experiences or exposure to toxins."
};

String[] Specific_PhobiasC = {
    "Genetic predisposition.",
    "Negative experiences or traumatic events related to the feared object or situation.",
    "Learned behaviors or associations."
};

String[] TrichotillomaniaC = {
    "Genetic predisposition.",
    "Psychological factors such as stress or anxiety.",
    "Environmental triggers such as boredom or tension."
};

        List<String[]> Causes = new ArrayList<>();

Causes.add(ADHD_C);
Causes.add(AgoraphobiaC);
Causes.add(Anorexia_NervosaC);
Causes.add(Antisocial_PersonalityC);
Causes.add(ASD_C);
Causes.add(Binge_EatingC);
Causes.add(Bipolar_DisorderC);
Causes.add(Borderline_PersonalityC);
Causes.add(Bulimia_NervosaC);
Causes.add(Dependent_PersonalityC);
Causes.add(DepressionC);
Causes.add(Dissociative_IdentityC);
Causes.add(ExcoriationC);
Causes.add(Generalized_AnxietyC);
Causes.add(Hoarding_DisorderC);
Causes.add(HypersomnolenceC);
Causes.add(InsomniaC);
Causes.add(Intellectual_DisabilityC);
Causes.add(Narcissistic_PersonalityC);
Causes.add(Obsessive_CompulsiveC);
Causes.add(Panic_DisorderC);
Causes.add(Paranoid_PersonalityC);
Causes.add(Post_TraumaticC);
Causes.add(Schizoid_PersonalityC);
Causes.add(Schizotypal_PersonalityC);
Causes.add(SchizophreniaC);
Causes.add(Social_AnxietyC);
Causes.add(Specific_LearningC);
Causes.add(Specific_PhobiasC);
Causes.add(TrichotillomaniaC);

        return Causes.get(n);
    }
    
    public static String[] Treatment(int n) {
        String[] ADHD_T = {
    "Stimulant medications such as methylphenidate or amphetamines.",
    "Behavioral therapy to learn coping strategies and improve organizational skills.",
    "Parent training and support to manage behavior at home.",
    "Education accommodations and support services."
};

String[] AgoraphobiaT = {
    "Cognitive-behavioral therapy (CBT) to address negative thought patterns and develop coping strategies.",
    "Exposure therapy to gradually confront feared situations or environments.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or benzodiazepines to reduce symptoms of anxiety.",
    "Support groups and self-help techniques."
};

String[] Anorexia_NervosaT = {
    "Nutritional counseling and meal planning to restore healthy eating patterns.",
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or family-based therapy (FBT), to address underlying emotional issues.",
    "Medical monitoring and management of physical health complications.",
    "Support groups and peer support networks."
};

String[] Antisocial_PersonalityT = {
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or dialectical behavior therapy (DBT), to address problematic behaviors and develop empathy.",
    "Medications for co-occurring conditions such as depression or anxiety.",
    "Family therapy to improve communication and address family dynamics.",
    "Community-based interventions and social support services."
};

String[] ASD_T = {
    "Behavioral therapy such as applied behavior analysis (ABA) or social skills training.",
    "Speech and language therapy to improve communication skills.",
    "Occupational therapy to address sensory sensitivities and motor skills.",
    "Educational accommodations and support services."
};

String[] Binge_EatingT = {
    "Cognitive Behavioral Therapy (CBT) to address thoughts and behaviors related to binge eating.",
    "Interpersonal Psychotherapy (IPT) to improve interpersonal relationships and address emotional triggers.",
    "Dialectical Behavior Therapy (DBT) to enhance emotion regulation and impulse control.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) may be prescribed in some cases."
};

String[] Bipolar_DisorderT = {
    "Mood stabilizers like lithium, anticonvulsants, or atypical antipsychotics to manage mood swings.",
    "Psychotherapy, including cognitive-behavioral therapy (CBT), psychoeducation, or family therapy.",
    "Medications for managing specific symptoms, such as antidepressants for depressive episodes or antipsychotics for manic episodes.",
    "Lifestyle adjustments such as maintaining a regular sleep schedule, avoiding alcohol and drugs, and seeking support from loved ones."
};

String[] Borderline_PersonalityT = {
    "Dialectical behavior therapy (DBT) to learn emotion regulation and interpersonal skills.",
    "Cognitive-behavioral therapy (CBT) to challenge and reframe distorted thinking patterns.",
    "Medications for co-occurring conditions such as depression or anxiety.",
    "Supportive relationships and structured routines."
};

String[] Bulimia_NervosaT = {
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or dialectical behavior therapy (DBT), to address distorted eating behaviors and body image concerns.",
    "Nutritional counseling and meal planning to establish regular eating patterns.",
    "Medications such as antidepressants to manage co-occurring symptoms of depression or anxiety.",
    "Support groups and self-help strategies."
};

String[] DepressionT = {
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or interpersonal therapy (IPT), to address negative thought patterns and develop coping strategies.",
    "Medications, including antidepressants like selective serotonin reuptake inhibitors (SSRIs) or serotonin-norepinephrine reuptake inhibitors (SNRIs).",
    "Lifestyle changes, such as regular exercise, healthy diet, and sufficient sleep.",
    "Support groups and self-help strategies."
};

String[] Dependent_PersonalityT = {
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or dialectical behavior therapy (DBT), to promote independence and self-esteem.",
    "Assertiveness training to develop confidence in decision-making and problem-solving.",
    "Group therapy or support groups to foster independence and reduce reliance on others.",
    "Developing a support network outside of dependent relationships."
};

String[] Dissociative_IdentityT = {
    "Psychotherapy, particularly trauma-focused therapy or dialectical behavior therapy (DBT).",
    "Medications for co-occurring conditions such as depression or anxiety.",
    "Integration therapy to help unify different identity states.",
    "Supportive relationships and validation of experiences."
};

String[] ExcoriationT = {
    "Cognitive-behavioral therapy (CBT), particularly habit reversal training (HRT), to identify triggers and develop alternative coping strategies.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or n-acetylcysteine (NAC) to reduce urges to pick skin.",
    "Skin care routines and protective measures to minimize damage from picking.",
    "Support groups and peer support networks for individuals with excoriation disorder."
};

String[] Generalized_AnxietyT = {
    "Cognitive-behavioral therapy (CBT) to identify and challenge irrational thoughts and behaviors.",
    "Medications, such as selective serotonin reuptake inhibitors (SSRIs), serotonin-norepinephrine reuptake inhibitors (SNRIs), or benzodiazepines.",
    "Relaxation techniques like deep breathing, meditation, or yoga.",
    "Stress management strategies including time management and setting realistic goals."
};

String[] Hoarding_DisorderT = {
    "Cognitive-behavioral therapy (CBT), particularly exposure and response prevention (ERP) therapy, to challenge hoarding behaviors and reduce clutter.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or tricyclic antidepressants to address underlying anxiety or depression.",
    "Home visits and practical interventions to help organize and declutter living spaces.",
    "Support groups and peer support networks for individuals and families affected by hoarding disorder."
};

String[] HypersomnolenceT = {
    "Stimulant medications such as modafinil or armodafinil to promote wakefulness during the day.",
    "Scheduled naps and strategic caffeine use to manage excessive sleepiness.",
    "Lifestyle adjustments such as maintaining a regular sleep schedule and improving sleep hygiene.",
    "Behavioral therapy to address underlying sleep disorders or habits."
};

String[] InsomniaT = {
    "Cognitive-behavioral therapy for insomnia (CBT-I) to address underlying sleep disturbances and improve sleep habits.",
    "Medications such as sedative-hypnotics or melatonin supplements, used short-term under medical supervision.",
    "Sleep hygiene education and lifestyle adjustments to promote better sleep.",
    "Relaxation techniques and stress management strategies."
};

String[] Intellectual_DisabilityT = {
    "Individualized educational programs (IEPs) tailored to the person's specific learning needs.",
    "Specialized educational support and accommodations in school settings.",
    "Speech and language therapy to improve communication skills.",
    "Occupational therapy to develop adaptive skills and independence in daily activities.",
    "Behavioral therapy to address challenging behaviors and develop social skills.",
    "Community-based services and support networks to enhance inclusion and quality of life."
};

String[] Narcissistic_PersonalityT = {
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or psychodynamic therapy, to explore underlying emotions and develop empathy.",
    "Group therapy to learn from others and receive feedback on interpersonal behavior.",
    "Medications for co-occurring conditions such as depression or anxiety.",
    "Self-help strategies and techniques for managing relationships."
};

String[] Obsessive_CompulsiveT = {
    "Cognitive-behavioral therapy (CBT), particularly exposure and response prevention (ERP) therapy.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or tricyclic antidepressants.",
    "Mindfulness techniques and relaxation exercises.",
    "Support groups and peer support networks."
};

String[] Panic_DisorderT = {
    "Cognitive-behavioral therapy (CBT) to challenge and restructure irrational thoughts and beliefs.",
    "Exposure therapy to gradually expose individuals to feared situations or sensations.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs), benzodiazepines, or antidepressants.",
    "Deep breathing exercises and relaxation techniques to manage panic symptoms."
};

String[] Paranoid_PersonalityT = {
    "Psychotherapy, such as cognitive-behavioral therapy (CBT) or psychodynamic therapy, to explore underlying fears and beliefs.",
    "Medications for co-occurring conditions such as anxiety or depression.",
    "Group therapy or support groups to develop trust and social skills.",
    "Coping strategies and stress management techniques."
};

String[] Post_TraumaticT = {
    "Trauma-focused therapies such as cognitive processing therapy (CPT) or eye movement desensitization and reprocessing (EMDR).",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or prazosin for nightmares and sleep disturbances.",
    "Mindfulness-based stress reduction techniques.",
    "Supportive relationships and social support networks."
};

String[] Schizoid_PersonalityT = {
    "Psychotherapy, particularly cognitive-behavioral therapy (CBT) or psychodynamic therapy, to explore emotions and social interactions.",
    "Social skills training to improve communication and relationship-building.",
    "Supportive environments that respect and accommodate individual preferences for solitude.",
    "Creative outlets and hobbies that provide fulfillment and expression."
};

String[] Schizotypal_PersonalityT = {
    "Psychotherapy, particularly cognitive-behavioral therapy (CBT) or dialectical behavior therapy (DBT), to challenge distorted thinking patterns and improve social skills.",
    "Medications for co-occurring conditions such as anxiety or depression.",
    "Social skills training and role-playing exercises to improve interpersonal interactions.",
    "Mindfulness and stress reduction techniques to manage anxiety and distress."
};

String[] SchizophreniaT = {
    "Antipsychotic medications to manage symptoms such as hallucinations and delusions.",
    "Psychosocial interventions such as cognitive-behavioral therapy (CBT), supportive therapy, or family therapy.",
    "Rehabilitation programs to improve social and vocational skills.",
    "Community support services and housing assistance."
};

String[] Social_AnxietyT = {
    "Cognitive-behavioral therapy (CBT) to address negative thought patterns and develop coping strategies.",
    "Exposure therapy to gradually confront feared social situations.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or beta blockers to reduce symptoms of anxiety.",
    "Support groups and self-help techniques."
};

String[] Specific_LearningT = {
    "Specialized educational interventions such as individualized education plans (IEPs) or accommodations.",
    "Remedial programs targeting specific areas of difficulty such as reading or math.",
    "Behavioral therapy to address emotional and behavioral challenges related to learning disabilities.",
    "Supportive environments and advocacy for educational needs."
};

String[] Specific_PhobiasT = {
    "Exposure therapy to gradually confront and desensitize individuals to the feared object or situation.",
    "Cognitive-behavioral therapy (CBT) to challenge and restructure irrational thoughts and beliefs.",
    "Medications such as beta blockers to reduce physical symptoms of anxiety during exposure.",
    "Relaxation techniques and mindfulness exercises."
};

String[] TrichotillomaniaT = {
    "Cognitive-behavioral therapy (CBT), particularly habit reversal training (HRT), to identify triggers and develop alternative coping strategies.",
    "Medications such as selective serotonin reuptake inhibitors (SSRIs) or n-acetylcysteine (NAC) to reduce urges to pull hair.",
    "Stress management techniques and relaxation exercises to reduce tension and anxiety.",
    "Support groups and peer support networks for individuals with trichotillomania."
};

        List<String[]> Treatments = new ArrayList<>();

Treatments.add(ADHD_T);
Treatments.add(AgoraphobiaT);
Treatments.add(Anorexia_NervosaT);
Treatments.add(Antisocial_PersonalityT);
Treatments.add(ASD_T);
Treatments.add(Binge_EatingT);
Treatments.add(Bipolar_DisorderT);
Treatments.add(Borderline_PersonalityT);
Treatments.add(Bulimia_NervosaT);
Treatments.add(Dependent_PersonalityT);
Treatments.add(DepressionT);
Treatments.add(Dissociative_IdentityT);
Treatments.add(ExcoriationT);
Treatments.add(Generalized_AnxietyT);
Treatments.add(Hoarding_DisorderT);
Treatments.add(HypersomnolenceT);
Treatments.add(InsomniaT);
Treatments.add(Intellectual_DisabilityT);
Treatments.add(Narcissistic_PersonalityT);
Treatments.add(Obsessive_CompulsiveT);
Treatments.add(Panic_DisorderT);
Treatments.add(Paranoid_PersonalityT);
Treatments.add(Post_TraumaticT);
Treatments.add(Schizoid_PersonalityT);
Treatments.add(Schizotypal_PersonalityT);
Treatments.add(SchizophreniaT);
Treatments.add(Social_AnxietyT);
Treatments.add(Specific_LearningT);
Treatments.add(Specific_PhobiasT);
Treatments.add(TrichotillomaniaT);

        return Treatments.get(n);
    }
    
    public static String DisorderNames(int n) {
        String[] Names = {
    "ADHDS",
    "AgoraphobiaS",
    "Anorexia_NervosaS",
    "Antisocial_PersonalityS",
    "Autism_Spectrum_DisorderS",
    "Binge_EatingS",
    "Bipolar_DisorderS",
    "Borderline_PersonalityS",
    "Bulimia_NervosaS",
    "Dependent_PersonalityS",
    "DepressionS",
    "Dissociative_IdentityS",
    "ExcoriationS",
    "Generalized_AnxietyS",
    "Hoarding_DisorderS",
    "HypersomnolenceS",
    "InsomniaS",
    "Intellectual_DisabilityS",
    "Narcissistic_PersonalityS",
    "Obsessive_CompulsiveS",
    "Panic_DisorderS",
    "Paranoid_PersonalityS",
    "Post_Traumatic_StressS",
    "Schizoid_PersonalityS",
    "Schizotypal_PersonalityS",
    "SchizophreniaS",
    "Social_AnxietyS",
    "Specific_LearningS",
    "Specific_PhobiasS",
    "TrichotillomaniaS"
};

        return Names[n];
    }
    public static String Questions(int n, Scanner sc) {
        String N = "None";
        int c = 0;
        String[][] S = Symptom(n);

        for (int k = 0; k < 4; k++) {
            System.out.println(S[k][0] + " : ");
            S[k][1] = sc.next();
            if (!S[k][1].equalsIgnoreCase("Y")) {
                c++;
            }
            if (c == 2) {
                break;
            }
        }
        if (c <= 1) 
        {
            
            N = DisorderNames(n);
            
            return N;
        }
        return N;
    }

    public static void main(String[] args) 
    {
        int k = 0;
        String N="";

        Scanner sc = new Scanner(System.in);
        
        System.out.println("Please fill out the following information:");
        System.out.print("Name: ");
        String name = sc.nextLine();
        
        System.out.print("Age: ");
        int age = sc.nextInt();
        
        System.out.println("\nMental Disorder Symptoms:");
        System.out.println("Please answer with 'Y' for Yes and 'N' for No : \n");

        for (k = 0; k < 30; k++) 
        {
            N = Questions(k,sc);
            
            if (N!="None") 
            {
                String[] C = Cause(k);
                String[] T = Treatment(k);
                System.out.println("\nSummary:");
                System.out.println("Name: " + name);
                System.out.println("Age: " + age);
                System.out.println("--------------------------------------------------------------------");
                System.out.println("For given Symptoms that you are Experiencing\n ");
                System.out.println(N + " Can be a disorder \n");
                System.out.println("Could be Cused Due to : ");
                for (String element : C) 
                {
                    System.out.println(element);
                }
                System.out.println("--------------------------------------------------------------------");
                System.out.println("\nTreatments could be : ");
                for (String element : T) 
                {
                    System.out.println(element);
                }
                System.out.println("\n\nFor further evolution Please contacnt a doctor ");
                break;
            }
        }
        if(N=="None")
        {
            System.out.println("\nSummary:");
            System.out.println("Name: " + name);
            System.out.println("Age: " + age);
            System.out.println("--------------------------------------------------------------------");
            System.out.println("Sorry , But none of your Symptoms match Our Database for a mental Disorder ");
            System.out.println("For further evolution Please contacnt a doctor ");
        }
        
        // To sve all data in Disorder List
        List<Object> Disorders = new ArrayList<>();
        
        for (int k = 0; k < 3; k++) 
        {
            List<Object> D = new ArrayList<>();
            String N = DisorderNames(k);
            String[][] S = Symptom(k);
            String[] C = Cause(k);
            String[] T = Treatment(k);
            D.add(N);
            D.add(S);
            D.add(C);
            D.add(T);
            Disorders.add(D);
            
        }
        for (Object obj : Disorders) 
        {
            List<Object> disorder = (List<Object>) obj;
            System.out.println(disorder.get(0)); 
            
            System.out.println("Symptoms : "); 
            String[][] symptoms = (String[][]) disorder.get(1);
            for (String[] symptom : symptoms) 
            {
                System.out.println(symptom[0] + " : " + symptom[1]);
                
            }
            
            System.out.println("Causes:");
            String[] causes = (String[]) disorder.get(2);
            for (String cause : causes) {
                System.out.println(cause);
            }

            System.out.println("Treatment:");
            String[] treatments = (String[]) disorder.get(3);
            for (String treatment : treatments) {
                System.out.println(treatment);
            }
            System.out.println();
        
    }
}
