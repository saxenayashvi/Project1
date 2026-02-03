# Project
import streamlit as st

# ---------------- PAGE CONFIG ----------------
st.set_page_config(
    page_title="BI4BI - EY Landing Page",
    layout="wide"
)

# ---------------- EY THEME CSS ----------------
st.markdown("""
<style>

    /* Full background */
    .stApp {
        background-color: white;
        font-family: "Segoe UI", sans-serif;
    }

    /* Remove Streamlit padding */
    section.main > div {
        padding-top: 30px;
    }

    /* Card Styling */
    .card {
        background: #ffffff;
        padding: 60px 70px;
        border-radius: 28px;
        box-shadow: 0px 8px 30px rgba(0,0,0,0.15);
        width: 850px;
        margin: auto;
        text-align: center;
    }

    /* BI4BI Title */
    .title {
        font-size: 55px;
        font-weight: 700;
        color: #333333;
        margin-bottom: 25px;
    }

    /* Description Text */
    .desc {
        font-size: 18px;
        color: #666666;
        line-height: 1.6;
        margin-bottom: 45px;
    }

    /* Button Styling */
    div.stButton > button {
        background-color: #FFD100;
        color: black;
        font-size: 20px;
        font-weight: 600;
        padding: 14px 160px;
        border-radius: 14px;
        border: none;
        box-shadow: 0px 6px 18px rgba(0,0,0,0.18);
        transition: 0.25s;
    }

    div.stButton > button:hover {
        background-color: #ffcc00;
        transform: scale(1.03);
    }

    /* Footer */
    .footer {
        margin-top: 35px;
        font-size: 14px;
        color: #999999;
    }

</style>
""", unsafe_allow_html=True)


# ---------------- HEADER ----------------
col1, col2 = st.columns([7, 2])

with col1:
    st.markdown("<h2>BI4BI <span style='font-weight:400;'>- EY Landing Page</span></h2>",
                unsafe_allow_html=True)

with col2:
    st.image(
        "https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/EY_logo_2019.svg/2560px-EY_logo_2019.svg.png",
        width=130
    )

st.markdown("<br><br>", unsafe_allow_html=True)


# ---------------- MAIN CARD ----------------
st.markdown("""
<div class="card">

    <div class="title">BI4BI</div>

    <div class="desc">
        BI4BI helps analyze existing BI reports, identify redundancies,<br>
        and provide recommendations to rationalize and modernize<br>
        legacy BI environments using metadata-driven insights.
    </div>

</div>
""", unsafe_allow_html=True)


# Button Centered
st.markdown("<br>", unsafe_allow_html=True)
col_btn1, col_btn2, col_btn3 = st.columns([3, 2, 3])

with col_btn2:
    st.button("Begin")


# ---------------- FOOTER ----------------
st.markdown("""
<div class="footer" style="text-align:center;">
©️ 2024 EYGM Limited. All Rights Reserved.
</div>
""", unsafe_allow_html=True)
